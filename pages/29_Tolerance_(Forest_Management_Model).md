# Tolerance (Forest Management Model)

In 1911 Raphael Zon and Henry Graves published an article called _Light in Relation to Tree Growth_[^Light_in_Relation_to_Tree_Growth]. This article details the methods that were used to classify species into tolerance categories. However, some researchers did not agree that light was the driving factor. In response, Frederick Baker published _A Revised Tolerance Table_[^A_Revised_Tolerance_Table] (1949) in which the real modification was the addition of more merchantable species of trees.  Along this same theme, Dr. James D. Arney used these 'tolerance tables' in the early 1990’s to determine regeneration in the Forest Projection and Planning System (FPS). (Arney et al, 2004)

The approach that Arney used was based on stem mapped permanent plot data. Since FPS is an individual tree, distance dependent model, tree level data could be used to calculate competition. Part of the calibration of this model was to look at the crown ratio for a tree with a competition level of 300 competitive stress index (CSI) (Arney, 1978). A level of 300 was chosen as it has been determined to approximate the beginning of the zone of imminent mortality in some species of conifers.

The Arney approach will work and has been demonstraited in FPS this model will use the same concept only inverted.  The tolerance value will be the CSI at a crown ratio of 20% (or other tested ratio).  The rationale for this method is to not assume that mortality begins at 300 CSI.  if it can be agreed that a tree is facing immenent mortality when the crown has receeded to 20% the resulting CSI should more precisely represent the exact tolerance status.  another advantage of this is from the field perspective one could see a crown of 20% and relate that to an estimated CSI.  While it will be of interest to evaluate other CR values as the critical threshold it may be determined that a matrix of CSI at given CR could prove to be useful for other modeling aspects.

``` text
 SPP\CR .1  .2  .3  .4  .5  .6  .7  .8  .9  1.0
 DF
 PP
 LP
 WH
 SS                   CSI values
 .
 .
 .
 XX
```

this methodology should be expanded to non tree vegetation also.  however the X axis would thange to % cover.

``` text
 SPP\%Cover .1  .2  .3  .4  .5  .6  .7  .8  .9  1.0
 GR
 SH
 BU
 OT                   CSI values
 .
 .
 .
 XX
```

## Notes

## Sources

[^Light_in_Relation_to_Tree_Growth]: [Zon, Raphael, and Graves, Henry S., Light in relation to tree growth.  U.S. Dept. Agric., Forest Service, Bull 92. pp.59. 1911.](https://archive.org/details/lightinrelationt92zonr)

[^A_Revised_Tolerance_Table]: [Baker, F.S. 1949. A revised tolerance table. J. For. 47, 179-181.](http://www.ingentaconnect.com/content/saf/jof/1949/00000047/00000003/art00005)

[[Category:Biometric_Principals_(Forest_Management_Model)]]
