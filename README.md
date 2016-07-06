# Geoserver SLDs!
Some SLD's I have been creating for features hosted on our Geoshape instance, via Geoserver. When serving features out of Geoserver via WMS, or for use in GeoNode/Geoshape, symbology can be set at the server level using SLD's so that the features are accessed by the end user while already symbolized accordingly. Though these SLD's are coded specifically for my features, I am providing the code here, because they may be useful to others as templates for their own work. 

Below is a snippet of what one rule of an SLD code looks like, in this case we are defining a specific attribute, by color. 

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

Some great online help resources as you work through styling your own SLD's:
GeoServer SLD Cookbook - http://docs.geoserver.org/stable/en/user/styling/sld-cookbook/
GeoSolutions Styling with SLD - http://geoserver.geo-solutions.it/edu/en/pretty_maps/styling.html

