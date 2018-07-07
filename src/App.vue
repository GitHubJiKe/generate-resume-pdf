<template>
  <div id="app">
    <button style="float:right;" @click="exportPdf">一键导出PDF</button>
    <router-view/>
  </div>
</template>

<script>
import html2pdf from 'html2pdf.js'
export default {
  name: 'App',
  methods: {
    exportPdf: function () {
      html2pdf(document.getElementById('resume'), {
        margin: [0, 1],
        filename: 'resume.pdf',
        image: {
          type: 'jpeg',
          quality: '0.99'
        },
        html2canvas: {
          dpi: 192,
          letterRendering: true
        },
        jsPDF: {
          unit: 'in',
          format: 'letter',
          orientation: 'portrait'
        }
      })
    }
  }
}
</script>

<style>
#app {
  padding: 0px 20px;
}
</style>
