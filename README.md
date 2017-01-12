# DataViz
Here is a project of visualizing French "ligue 1" ranking.
This is the code of the visualization.

<!DOCTYPE html>
<meta charset="utf-8">
    
    
    <style>
        
        body { font: 14px Arial;}
        
        path {
            stroke: steelblue;
            stroke-width: 2;
            fill: none;
        }
    
    .axis path,
    .axis line {
        fill: none;
        stroke: grey;
        stroke-width: 1;
        shape-rendering: crispEdges;
    }
    
    .legend {
        font-size: 12px;
        font-weight: bold;
        text-anchor: middle;
    }
    
        </style>
    
    
    
    <body>
        
        <script src="http://d3js.org/d3.v3.min.js"></script>
        
        <script>
            
            // Définir les dimensions de la page
            var margin = {top: 80, right: 320, bottom: 120, left: 50},
            width = 1000 - margin.left - margin.right +290,
            height = 500 - margin.top - margin.bottom + 100;
            
            // Parser les dates
            var parseDate = d3.time.format("%b %d %Y").parse;
            
            // Définir les échelles
            var x = d3.time.scale().range([0, width]);
            var y = d3.scale.linear().range([0, height]);
            
            // Définir les axes
            var xAxis = d3.svg.axis().scale(x)
            .orient("bottom").ticks(10);
            
            var yAxis = d3.svg.axis().scale(y)
            .orient("left").ticks(20);
            
            // Définir les lignes
            var classementline = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.classement); })
            
            
            var classementline1 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred1); })
            
            
            
            var classementline2 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred2); })
            
            
            var classementline3 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred3); })
            
            
            var classementline4 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred4); })
            
            
            var classementline5 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred5); })
            
            
            var classementline6 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred6); })
            
            
            var classementline7 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred7); })
            
            
            var classementline8 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred8); })
            
            
            
            var classementline9 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred9); })
            
            
            var classementline10 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred10); })
            
            
            var classementline11 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred11); })
            
            
            var classementline12 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred12); })
            
            
            var classementline13 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred13); })
            
            
            var classementline14 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred14); })
            
            
            var classementline15 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred15); })
            
            
            var classementline16 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred16); })
            
            
            var classementline17 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred17); })
            
            
            var classementline18 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred18); })
            
            
            
            var classementline19 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred19); })
            
            
            var classementline20 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred20); })
            
            
            var classementline21 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred21); })
            
            
            var classementline22 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred22); })
            
            
            var classementline23 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred23); })
            
            
            var classementline24 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred24); })
            
            
            var classementline25 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred25); })
            
            
            var classementline26 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred26); })
            
            
            var classementline27 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred27); })
            
            
            var classementline28 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred28); })
            
            
            
            var classementline29 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred29); })
            
            
            var classementline30 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred30); })
            
            
            var classementline31 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred31); })
            
            
            var classementline32 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred32); })
            
            
            var classementline33 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred33); })
            
            
            var classementline34 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred34); })
            
            
            var classementline35 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred35); })
            
            
            var classementline36 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred36); })
            
            
            var classementline37 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred37); })
            
            
            var classementline38 = d3.svg.line()
            .x(function(d) { return x(d.date); })
            .y(function(d) { return y(d.pred38); })
            
            
            
            
            // Définition du SVG
            var svg = d3.select("body")
            .append("svg")
            .attr("width", width + margin.left + margin.right)
            .attr("height", height + margin.top + margin.bottom)
            .append("g")
            .attr("transform",
                  "translate(" + margin.left + "," + margin.top + ")");
                  
                  // Obtenir les données
                  d3.csv("stocks.csv", function(error, data) {
                         data.forEach(function(d) {
                                      d.date = parseDate(d.date);
                                      d.classement = +d.classement;
                                      });
                         console.log(d3.min(data, function(d) { return d.date; }))
                         // Définir le domaine en fonction des données
                         x.domain([d3.min(data, function(d) { return d.date; }),d3.max(data, function(d) { return d.date; })]);
                         y.domain([1, d3.max(data, function( d) { return d.classement; })+1]);
                         
                         // Parser par rapport au nom de l'équipe
                         var dataNest = d3.nest()
                         .key(function(d) {return d.equipe;})
                         .entries(data);
                         
                         // Définir le vecteur de couleurs
                         var color = d3.scale.category20();
                         
                         // Définir l'espace de la légende
                         legendSpace = width/dataNest.length;
                         
                         // Boucle sur toutes les clés qui sont les noms d'équipes
                         dataNest.forEach(function(d,i) {
                                          
                                          // Ajouter les lignes
                                          svg.append("path")
                                          .attr("class", "line")
                                          .style("stroke", function() {
                                                 return d.color = color(d.key); })
                                          .attr("id", 'tag'+d.key.replace(/\s+/g, ''))
                                          .attr("stroke-width", 2)
                                          .style("opacity", 0)
                                          .attr("d", classementline(d.values));
                                          
                                          svg.selectAll("rect")
                                          .data(data)
                                          .enter().append("rect")
                                          .attr("height",110)
                                          .attr("width",190)
                                          .attr("x", 1040)
                                          .attr("y", 0)
                                          .attr("rx", 10)
                                          .attr("ry", 10)
                                          .style("fill","White")
                                          .style("stroke-width",5)
                                          .style("opacity", 0);
                                          
                                          
                                          // Ajouter les points des équipes à chaque journée
                                          svg.selectAll(".value")
                                          .data(data)
                                          .enter().append("text")
                                          .text(function(d) { return "Journée:"+"\n"+d.journee;})
                                          .attr("class", "value")
                                          .attr("y", 14)
                                          .attr("x", 1050)
                                          .style("opacity", 0)
                                          .style("font-family", "monospace");
                                          
                                          svg.selectAll(".value2")
                                          .data(data)
                                          .enter().append("text")
                                          .text(function(d) { return "Equipe:"+"\n"+d.equipe;})
                                          .attr("class", "value")
                                          .attr("y", 29)
                                          .attr("x", 1050)
                                          .style("opacity", 0)
                                          .style("font-family", "monospace");
                                          
                                          svg.selectAll(".value3")
                                          .data(data)
                                          .enter().append("text")
                                          .text(function(d) { return "Points:"+"\n"+d.points;})
                                          .attr("class", "value")
                                          .attr("y", 44)
                                          .attr("x", 1050)
                                          .style("opacity", 0)
                                          .style("font-family", "monospace");
                                          
                                          svg.selectAll(".value4")
                                          .data(data)
                                          .enter().append("text")
                                          .text(function(d) { return "Classement:"+"\n"+d.classement;})
                                          .attr("class", "value")
                                          .attr("y", 59)
                                          .attr("x", 1050)
                                          .style("opacity", 0)
                                          .style("font-family", "monospace");
                                          
                                          svg.selectAll(".value5")
                                          .data(data)
                                          .enter().append("text")
                                          .text( function(d) { return"AIC:"+"\n"+d.aic;})
                                          .attr("class", "value")
                                          .attr("y", 74)
                                          .attr("x", 1050)
                                          .style("opacity", 0)
                                          .style("font-family", "monospace");
                                          
                                          svg.selectAll(".value6")
                                          .data(data)
                                          .enter().append("text")
                                          .text("Average AIC:32")
                                          .attr("class", "value")
                                          .attr("y", 89)
                                          .attr("x", 1050)
                                          .style("opacity", 0)
                                          .style("font-family", "monospace");
                                          
                                          svg.selectAll(".value7")
                                          .data(data)
                                          .enter().append("text")
                                          .text(function(d) { if(d.aic<32){return "bon modèle"} else{return "mauvais modèle"};})
                                          .attr("class", "value")
                                          .attr("y", 104)
                                          .attr("x", 1050)
                                          .style("opacity", 0)
                                          .style("font-family", "monospace");
                                          
                                          
                                          
                                          
                                          
                                          // Ajouter le nom des équipes pour la dernière journée à droite
                                          svg.selectAll("equipes")
                                          .data(data)
                                          .enter()
                                          .append("a")
                                          .attr("xlink:href", function(d){if(d.journee==38){return d.url}})
                                          .attr("target", "_blank")
                                          .append("text").text(function(d) {
                                                               if(d.journee==38){ return d.equipe;}})
                                          .attr("y", function(d) {
                                                return y(d.classement)+3; })
                                          .attr("x", function(d) {
                                                return x(d.date)+20;})
                                          .style("opacity", 1);
                                          
                                          
                                          // Ajouter les points
                                          svg.selectAll("dot")
                                          .data(d.values)
                                          .enter().append("circle")
                                          .attr("r", 2)
                                          .attr("cx", function(d) { return x(d.date); })
                                          .attr("cy", function(d) { return y(d.classement); })
                                          .style("opacity", 1)
                                          .on("mouseover", function(g) {
                                              d3.select(this).attr("r", 5).style("fill", "blue")
                                              d3.selectAll(".value").filter(function(e) {
                                                                            return g === e;
                                                                            })
                                              .style("opacity",1);
                                              d3.selectAll("rect").style("opacity",1)
                                              .style("stroke",function() {
                                                     return d.color = color(d.key); });
                                              
                                              
                                              if(g.journee==1){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline1(d.values))
                                              .style("stroke-dasharray", ("3, 3"))
                                              ;}
                                              
                                              
                                              if(g.journee==2){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline2(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==3){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline3(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==4){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline4(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==5){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline5(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==6){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline6(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==7){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline7(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==8){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline8(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==9){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline9(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==10){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline10(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==11){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline11(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==12){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline12(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==13){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline13(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==14){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline14(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==15){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline15(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==16){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline16(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==17){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline17(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==18){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline18(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==19){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline19(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==20){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline20(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==21){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline21(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==22){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline22(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==23){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline23(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==24){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline24(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==25){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline25(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==26){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline26(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==27){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline27(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==28){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline28(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==29){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline29(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==30){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline30(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==31){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline31(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==32){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline32(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==33){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline33(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==34){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline34(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==35){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline35(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==36){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline36(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==37){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline37(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              
                                              if(g.journee==38){
                                              svg.append("path")
                                              .attr("class", "line1")
                                              .style("stroke", function() {
                                                     return d.color = color(d.key); })
                                              .attr("d", classementline38(d.values))
                                              .style("stroke-dasharray", ("3, 3"));}
                                              })
                                          
                                          .on("mouseout", function(d){
                                              d3.select(this).attr("r", 2).style("fill", "black")
                                              d3.selectAll(".value").filter(function(e) {
                                                                            return d === e;
                                                                            })
                                              .style("opacity",0);
                                              svg.selectAll(".line1").remove()
                                              d3.selectAll("rect").style("opacity",0);})
                                          
                                          
                                          //Ajouter la légende
                                          
                                          if(i<10){
                                          svg.append("text")
                                          .attr("x",(((i+1)*100-80)))
                                          .attr("y", height + (margin.bottom/2)+ 5)
                                          .attr("class", "legend")
                                          .style("fill", function() {
                                                 return d.color = color(d.key); })
                                          .on("click", function(){
                                              var active   = d.active ? false : true,
                                              newOpacity = active ? 1 : 0;
                                              d3.select("#tag"+d.key.replace(/\s+/g, ''))
                                              .transition().duration(100)
                                              .style("opacity", newOpacity);
                                              d.active = active;
                                              })
                                          .text(d.key);
                                          }
                                          else{
                                          svg.append("text")
                                          .attr("x", ((i-9)*100-80))
                                          .attr("y", height + (margin.bottom/2)+30)
                                          .attr("class", "legend")
                                          .style("fill", function() {
                                                 return d.color = color(d.key); })
                                          .on("click", function(){
                                              var active   = d.active ? false : true,
                                              newOpacity = active ? 0 : 1;
                                              d3.select("#tag"+d.key.replace(/\s+/g, ''))
                                              .transition().duration(100)
                                              .style("opacity", newOpacity);
                                              d.active = active;
                                              })
                                          .text(d.key);
                                          }
                                          });
                         
                         // Ajouter l'axe des X
                         svg.append("g")
                         .attr("class", "x axis")
                         .attr("transform", "translate(0," + height + ")")
                         .call(xAxis);
                         
                         // Ajouter l'axe des Y
                         svg.append("g")
                         .attr("class", "y axis")
                         .attr("transform", "translate(" + -10 + "," + -1 + ")")
                         .call(yAxis);
                         
                         // Ajouter le titre
                         svg.append("text")
                         .attr("x", (width / 2)+50)
                         .attr("y", -40 )
                         .attr("text-anchor", "middle")
                         .style("font-size", "18px")
                         .attr("fill","black")
                         .text(" Classements et prédictions de la Ligue 1");
                         
                         
                         });
                         
            </script>
    </body>



