# Geoserver_SLD-s
Some SLD's I have been creating for features hosted on our Geoshape instance, via Geoserver. 

Below is a snippet of what part of SLD code looks like... 

```<Rule>
<Name>PI Low - MPI Low</Name>
<Title>PI Low - MPI Low</Title>
<ogc:Filter>
<ogc:PropertyIsEqualTo>
<ogc:PropertyName>Bi_Class</ogc:PropertyName>
<ogc:Literal>A1</ogc:Literal>
</ogc:PropertyIsEqualTo>
</ogc:Filter>
<PolygonSymbolizer>
<Fill>
<CssParameter name="fill">#e8e8e8</CssParameter>
</Fill>
<Stroke>
<CssParameter name="stroke">#000000</CssParameter>
<CssParameter name="stroke-width">0.26</CssParameter>
<CssParameter name="stroke-linejoin">bevel</CssParameter>
</Stroke>
</PolygonSymbolizer>
</Rule>
```
And below is an example of the output...
<p align="center">
  <img src="Geoserver_SLD-s/SLD_ExampleOutput.png="350"/>
  <img src="Geoserver_SLD-s/SLD_ExampleOutput.png" width="350"/>
</p>
