---
title: Erin's Interactive Thesis
description: A sampling of interactive data visualizations created throughout my PhD research.
---

# Motif information content vs. promoter region enrichment for consensus predictions derived from the computational promoter ID framework

### Interactive plot instructions:
* Hover over points and lines for more information about each motif
* Click+drag mouse to pan
* Use scroll wheel to zoom

{::nomarkdown}
<!DOCTYPE html>
<html>
<head>
  <style>
    .error {
        color: red;
    }
  </style>
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm//vega@5"></script>
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm//vega-lite@4.17.0"></script>
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm//vega-embed@6"></script>
</head>
<body>
  <div id="vis"></div>
  <script>
    (function(vegaEmbed) {
      var spec = {"config": {"view": {"continuousWidth": 400, "continuousHeight": 300}, "axis": {"grid": false, "labelFontSize": 14, "titleFontSize": 18}}, "layer": [{"mark": {"type": "circle", "opacity": 0.5, "size": 500}, "encoding": {"color": {"type": "nominal", "field": "org", "scale": {"scheme": "Set2"}, "title": "Organism"}, "tooltip": [{"type": "ordinal", "field": "nperc"}, {"type": "quantitative", "field": "enrich_ratio"}, {"type": "quantitative", "field": "motif_ave_ic"}, {"type": "nominal", "field": "m1"}, {"type": "nominal", "field": "m2"}], "x": {"type": "quantitative", "field": "motif_ave_ic", "title": "Motif Average Positional Information Content"}, "y": {"type": "quantitative", "field": "enrich_ratio", "title": "Promoter Enrichment Ratio"}}}, {"mark": {"type": "text", "align": "center", "baseline": "middle", "color": "black", "size": 14}, "encoding": {"text": {"type": "nominal", "field": "nperc"}, "tooltip": [{"type": "ordinal", "field": "nperc"}, {"type": "quantitative", "field": "enrich_ratio"}, {"type": "quantitative", "field": "motif_ave_ic"}, {"type": "nominal", "field": "m1"}, {"type": "nominal", "field": "m2"}], "x": {"type": "quantitative", "field": "motif_ave_ic"}, "y": {"type": "quantitative", "field": "enrich_ratio"}}, "height": 250, "selection": {"selector006": {"type": "interval", "bind": "scales", "encodings": ["x", "y"]}}, "width": 500}], "data": {"name": "data-bd7a341d91801d4854724d8ebddb867c"}, "$schema": "https://vega.github.io/schema/vega-lite/v4.0.2.json", "datasets": {"data-bd7a341d91801d4854724d8ebddb867c": [{"nperc": 1, "enrich_ratio": -0.19684135767056424, "motif_ave_ic": 0.7065553657616764, "m1": "AGCTTT", "m2": "GCAGCA", "org": "M. buryatense"}, {"nperc": 2, "enrich_ratio": 2.0466126791937134, "motif_ave_ic": 0.7445147996719239, "m1": "TTGATA", "m2": "TATAAT", "org": "M. buryatense"}, {"nperc": 3, "enrich_ratio": 2.007411229055583, "motif_ave_ic": 0.7733000295367951, "m1": "TTGACA", "m2": "TATAAT", "org": "M. buryatense"}, {"nperc": 4, "enrich_ratio": null, "motif_ave_ic": 0.3991651501452376, "m1": "TTGTTT", "m2": "TAAAAA", "org": "M. buryatense"}, {"nperc": 5, "enrich_ratio": 2.1174900600096045, "motif_ave_ic": 0.7065233924921394, "m1": "TTGACA", "m2": "TATAAT", "org": "M. buryatense"}, {"nperc": 6, "enrich_ratio": 1.9937236343850875, "motif_ave_ic": 0.573164119727333, "m1": "TTGTCA", "m2": "TAATAT", "org": "M. buryatense"}, {"nperc": 10, "enrich_ratio": 1.0295890869420934, "motif_ave_ic": 0.6190647591640334, "m1": "CTTGAT", "m2": "TGATAA", "org": "M. buryatense"}, {"nperc": 20, "enrich_ratio": 1.993239806185073, "motif_ave_ic": 0.49714786749753914, "m1": "GCTTAA", "m2": "GGTATA", "org": "M. buryatense"}, {"nperc": 1, "enrich_ratio": null, "motif_ave_ic": 0.6104727532411306, "m1": "GCTAAC", "m2": "TGAAGG", "org": "E. coli"}, {"nperc": 2, "enrich_ratio": null, "motif_ave_ic": 0.5130301143453476, "m1": "GTTTTT", "m2": "GGCGCA", "org": "E. coli"}, {"nperc": 3, "enrich_ratio": 1.0277512714651915, "motif_ave_ic": 0.6547198869332699, "m1": "ACCTCA", "m2": "TGTGGA", "org": "E. coli"}, {"nperc": 4, "enrich_ratio": null, "motif_ave_ic": 0.7011071144041697, "m1": "TATCCA", "m2": "TGAACG", "org": "E. coli"}, {"nperc": 5, "enrich_ratio": 1.8339908059562249, "motif_ave_ic": 0.4949958976243365, "m1": "TCTTCT", "m2": "CAGGAG", "org": "E. coli"}, {"nperc": 6, "enrich_ratio": null, "motif_ave_ic": 0.5406027164220665, "m1": "CTTACA", "m2": "CATGAA", "org": "E. coli"}, {"nperc": 7, "enrich_ratio": null, "motif_ave_ic": 0.46935218479816304, "m1": "CTTACA", "m2": "GATAAT", "org": "E. coli"}, {"nperc": 8, "enrich_ratio": 0.7560346225315969, "motif_ave_ic": 0.59486357337625, "m1": "TGCCAT", "m2": "TATAAT", "org": "E. coli"}, {"nperc": 9, "enrich_ratio": 1.1894422557612323, "motif_ave_ic": 0.5171640515654675, "m1": "TGCCAA", "m2": "TATAAT", "org": "E. coli"}, {"nperc": 10, "enrich_ratio": null, "motif_ave_ic": 0.33010212699118574, "m1": "TGCCAA", "m2": "TAGAAT", "org": "E. coli"}, {"nperc": 3, "enrich_ratio": 2.700579720712215, "motif_ave_ic": 0.8704647658213913, "m1": "TTGACA", "m2": "TATAAT", "org": "B. subtilis"}, {"nperc": 4, "enrich_ratio": null, "motif_ave_ic": 0.8829778133803402, "m1": "TTGACA", "m2": "TATAAT", "org": "B. subtilis"}, {"nperc": 5, "enrich_ratio": 2.7692325398563713, "motif_ave_ic": 0.9102310690178204, "m1": "TTGACA", "m2": "TATAAT", "org": "B. subtilis"}, {"nperc": 6, "enrich_ratio": null, "motif_ave_ic": 0.8965937998107641, "m1": "TTGACA", "m2": "TATAAT", "org": "B. subtilis"}, {"nperc": 7, "enrich_ratio": null, "motif_ave_ic": 0.9177395105231155, "m1": "TTGACA", "m2": "TATAAT", "org": "B. subtilis"}, {"nperc": 8, "enrich_ratio": 2.6002417375212494, "motif_ave_ic": 0.9287377715786977, "m1": "TTGACA", "m2": "TATAAT", "org": "B. subtilis"}, {"nperc": 9, "enrich_ratio": 2.651205566824997, "motif_ave_ic": 0.9205544998740246, "m1": "TTGACA", "m2": "TATAAT", "org": "B. subtilis"}, {"nperc": 10, "enrich_ratio": 2.627891117888205, "motif_ave_ic": 0.9427480127562579, "m1": "TTGACA", "m2": "TATAAT", "org": "B. subtilis"}]}};
      var embedOpt = {"mode": "vega-lite"};

      function showError(el, error){
          el.innerHTML = ('<div class="error" style="color:red;">'
                          + '<p>JavaScript Error: ' + error.message + '</p>'
                          + "<p>This usually means there's a typo in your chart specification. "
                          + "See the javascript console for the full traceback.</p>"
                          + '</div>');
          throw error;
      }
      const el = document.getElementById('vis');
      vegaEmbed("#vis", spec, embedOpt)
        .catch(error => showError(el, error));
    })(vegaEmbed);

  </script>
</body>
</html>
{:/}

### Figure description
Visualization to compare the quality of predicted motifs for different gene sets across different organisms. Each point is a predicted motif from _M. buryatense_, _E. coli_, or _B. subtilis_. The numerical label of each point is the n% gene set used to derive that motif. The x-axis represents the information content of each motif averaged across each of the 12 positions in the motif. The y-axis represents the log2 ratio of the frequency the motif was found <100bp from a gene start to the frequency the motif was found in intergenic regions. _B. subilitis_ predictions had the highest overall information content and enrichment in promoter regions, with _E. coli_ motif predictions resulting in lower information content and lower enrichment in promoter regions, consistent with findings from Latif _et al._ suggesting _E. coli_ promoters have higher variability relative to the consensus. The motif chosen for experimental follow up in _M. buryatense_, the top 3% motif, appears in between the results for _B. subtilis_ and _E. coli_ in each dimension.

<button onclick="location.href='https://erinhwilson.github.io/interactive-thesis'" 
        type="button">Return to Main Page
</button>
