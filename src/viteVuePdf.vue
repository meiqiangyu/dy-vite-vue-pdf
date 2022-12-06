<style src="./annotationLayer.css"></style>

<script>
import pdfjs            from 'duyansoft-pdfjs-dist/build/pdf';
import pdfjsWrapper     from './pdfjsWrapper';
import componentFactory from './componentFactory';
import pdfjsWorker      from './pdf.worker.min.js'
// pdfjs.GlobalWorkerOptions.workerSrc = 'https://cdn.jsdelivr.net/npm/pdfjs-dist@2.16.105/build/pdf.worker.min.js';
(typeof window !== "undefined"
  ? window
  : {}
).pdfjsWorker = pdfjsWorker
var component = componentFactory( pdfjsWrapper( pdfjs ) );
export default component;
</script>