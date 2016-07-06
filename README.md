# Geoserver Styled Layer Descriptors (SLDs)...
This is a space for SLD's I have been creating for features hosted on our Geoshape instance, via Geoserver. There are some excellent online resources for building your own linked at the bottom of this readme, but I figured I would start posting SLD's here for ease of use as other users might be looking for a template for their own features. Though these SLD's are coded specifically for some generic features, they should be easy to re-tool for your own features if you are just getting going with SLDs. 

Below is a snippet of what one rule in SLD code looks like, in this case we are defining a specific attribute, by color. Naturally this is done for each attribute you want to specify a rule for throughout the entire SLD.  

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

![Sample SLD Output](https://github.com/Nickgis/Geoserver_SLD-s/blob/master/SLD_ExampleOutput.png?raw=true "Sample")

<B>Some great online help resources as you work through styling your own SLD's:</B>
<br>
GeoServer SLD Cookbook - http://docs.geoserver.org/stable/en/user/styling/sld-cookbook/
<br>
GeoSolutions Styling with SLD - http://geoserver.geo-solutions.it/edu/en/pretty_maps/styling.html

