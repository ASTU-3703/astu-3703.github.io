Notes:

Had to remove: [['$', '$'],  from below in themes/reveal-hugo/layouts/partials/layout/javascript.html 

Mathjax was changing every $ to garabge.

<script>
  MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']]
    },
    svg: {
      fontCache: 'global'
    }
  };
</script>

Changed to:

      inlineMath: [['\\(', '\\)']]  // Changes inline math delimiter to \( and \)