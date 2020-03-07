<body>
#nodes
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
Mns nodes utility module. <br>
All node creation functions are covered by this module <br>
</font>
</i>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###adlNode
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>adlNode(input1 = None, input2 = None, output = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>input1</b>(<i>str</i>) ; [default: None]</li>
<li><b>input2</b>(<i>str</i>) ; [default: None]</li>
<li><b>output</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: addDoubleLinear] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###buildGeoAxisVis
<font color = #5f5f5f size = 3pt>
<i>
Utility aid function: <br>
Creates a Axis-Vis geometry object based on parameters <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildGeoAxisVis(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (created vis-geo object)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: pointsOnCurve] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
<li><b>scale</b>(<i>int</i>) ; [default: 1] - Relative to parent</li>
<li><b>axisSubdevision</b>(<i>int</i>) ; [default: 16] - Geometry cylinder axis subdevision</li>
<li><b>cylinderWidth</b>(<i>float</i>) ; [default: 0.015]</li>
<li><b>deleteAll</b>(<i>bool</i>) - If true, do not attempt to create any objects- instead look for any existing objects and delete them</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###buildGeoAxisVisForParents
<font color = #5f5f5f size = 3pt>
<i>
Utility aid function. <br>
Created an Axis-Vis geometry object from each object within the list passed in. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildGeoAxisVisForParents(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>parentObjs</b>(<i>list</i>) ; [default: [' ']] - If parent is empty, visGeo will not build</li>
<li><b>parentMethod</b>(<i>int</i>)</li>
<li><b>scale</b>(<i>int</i>) ; [default: 1] - Relative to parent</li>
<li><b>axisSubdevision</b>(<i>int</i>) ; [default: 16] - Geometry cylinder axis subdevision</li>
<li><b>cylinderWidth</b>(<i>float</i>) ; [default: 0.015]</li>
<li><b>createNodeRelationship</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###buildVisCubesForPSOCNode
<font color = #5f5f5f size = 3pt>
<i>
Single use function. <br>
From a given MnsPointsOnCurve node, create output 'visCubes'. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildVisCubesForPSOCNode(node = "", **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict ('visCubesStds': output MnsNameStd list, 'nodes': output node list )</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>node</b>(<i>str</i>) ; [default: ""]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>gapWidth</b>(<i>float</i>) ; [default: 0.1]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###choiceNode
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>choiceNode(inputs = [], output = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>inputs</b>(<i>list</i>) ; [default: []]</li>
<li><b>output</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: choice] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###conditionNode
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>conditionNode(firstTerm = None, secondTerm = None, colorIfTrue = None, colorIfFalse = None, outColor = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>firstTerm</b>(<i>str</i>) ; [default: None]</li>
<li><b>secondTerm</b>(<i>str</i>) ; [default: None]</li>
<li><b>colorIfTrue</b>(<i>str</i>) ; [default: None]</li>
<li><b>colorIfFalse</b>(<i>str</i>) ; [default: None]</li>
<li><b>outColor</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: condition] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>operation</b>(<i>int</i>)</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###connectAttrAttempt
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectAttrAttempt(attrA, nodeAttr)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>attrA</b></li>
<li><b>nodeAttr</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###connectSetAttempt
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectSetAttempt(attrA, nodeAttr, valType)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>attrA</b></li>
<li><b>nodeAttr</b></li>
<li><b>valType</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###imagePlaneNode
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>imagePlaneNode(camera = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>camera</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: imagePlane] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###mdNode
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mdNode(input1 = None, input2 = None, output = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>input1</b>(<i>str</i>) ; [default: None]</li>
<li><b>input2</b>(<i>str</i>) ; [default: None]</li>
<li><b>output</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: multDev] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>operation</b>(<i>int</i>) ; [default: 1]</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###mdlNode
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mdlNode(input1 = None, input2 = None, output = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>input1</b>(<i>str</i>) ; [default: None]</li>
<li><b>input2</b>(<i>str</i>) ; [default: None]</li>
<li><b>output</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: multDoubleLinear] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###mnsAnnotateNode
<font color = #5f5f5f size = 3pt>
<i>
Creates an mnsAnnotateNode node based on specified parameters and outputs. <br>
Input as a node.channel list. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mnsAnnotateNode(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> dict ('node': MnsNameStd)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: annotate] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
<li><b>attributes</b>(<i>list</i>) ; [default: [' ']]</li>
<li><b>nameOnlyMode</b>(<i>bool</i>)</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###mnsBuildTransformsCurveNode
<font color = #5f5f5f size = 3pt>
<i>
Creates an mnsBuildTransformsCurveNode node based on specified parameters and outputs. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mnsBuildTransformsCurveNode(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict ('transforms': input transforms list, 'outCurve': built output curve MnsNameStd, 'outOffsetCurve': built output up-curve MnsNameStd, 'node': Created node MnsNameStd)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: buildTransformsCurveCurve] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
<li><b>transforms</b>(<i>list</i>) ; [default: [' ']] - transforms to build the curve from</li>
<li><b>buildOffsetCurve</b>(<i>bool</i>) - Node's 'buildOffsetCurve' attribute</li>
<li><b>offsetCurveSuffix</b>(<i>str</i>) ; [default: Up] - Up curve creation name body suffix</li>
<li><b>buildMode</b>(<i>int</i>) - Node's buildMode attribute</li>
<li><b>tangentDirection</b>(<i>int</i>) - Node's tangentDirection attribute</li>
<li><b>tangentLength</b>(<i>float</i>) ; [default: 1.0] - Node's tangentLength attribute</li>
<li><b>hermiteSteps</b>(<i>int</i>) ; [default: 5] - Node's hermiteSteps attribute</li>
<li><b>degree</b>(<i>int</i>) ; [default: 3] - Node's degree attribute</li>
<li><b>offsetType</b>(<i>int</i>) - Node's offsetType attribute</li>
<li><b>offsetX</b>(<i>float</i>) - Node's offsetX attribute</li>
<li><b>offsetY</b>(<i>float</i>) - Node's offsetY attribute</li>
<li><b>offsetZ</b>(<i>float</i>) - Node's offsetZ attribute</li>
<li><b>reverse</b>(<i>bool</i>) - Node's reverse attribute</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###mnsCameraGateRatioNode
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mnsCameraGateRatioNode(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: cameraGateRatio] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
<li><b>camera</b>(<i>str</i>)</li>
<li><b>widthInput</b>(<i>str</i>)</li>
<li><b>heightInput</b>(<i>str</i>)</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###mnsIKSolver
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mnsIKSolver(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: ikSolver] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
<li><b>blend</b>(<i>float</i>)</li>
<li><b>roll</b>(<i>float</i>)</li>
<li><b>slide</b>(<i>float</i>)</li>
<li><b>softness</b>(<i>float</i>)</li>
<li><b>stretchLimit</b>(<i>float</i>) ; [default: 1.0]</li>
<li><b>aimAxis</b>(<i>int</i>) ; [default: 1] - Node's 'aimAxis' attribute</li>
<li><b>upAxis</b>(<i>int</i>) ; [default: 2] - Node's 'upAxis' attribute</li>
<li><b>boneLengthA</b>(<i>float</i>) ; [default: 1.0]</li>
<li><b>boneLengthB</b>(<i>float</i>) ; [default: 1.0]</li>
<li><b>rootPos</b>(<i>str</i>)</li>
<li><b>midPos</b>(<i>str</i>)</li>
<li><b>endPos</b>(<i>str</i>)</li>
<li><b>limbRoot</b>(<i>str</i>)</li>
<li><b>ikHandle</b>(<i>str</i>)</li>
<li><b>poleVector</b>(<i>str</i>)</li>
<li><b>outputRoot</b>(<i>str</i>)</li>
<li><b>outputMid</b>(<i>str</i>)</li>
<li><b>outputEnd</b>(<i>str</i>)</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###mnsMatrixConstraintNode
<font color = #5f5f5f size = 3pt>
<i>
Creates an mnsMatrixConstraintNode node based on specified parameters and outputs. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mnsMatrixConstraintNode(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict ('nameStds': Created MnsNameStd list)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: matrixConstraint] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
<li><b>targets</b>(<i>list</i>) ; [default: [' ']] - Tragets to constrain</li>
<li><b>sources</b>(<i>list</i>) ; [default: [' ']] - Sources to constrain the targets to</li>
<li><b>maintainOffset</b>(<i>bool</i>) - Node's maintainOffset attribute</li>
<li><b>connectTranslate</b>(<i>bool</i>) ; [default: True] - Connect Translate if True</li>
<li><b>connectRotate</b>(<i>bool</i>) ; [default: True] - Connect Rotate if True</li>
<li><b>connectScale</b>(<i>bool</i>) ; [default: True] - Connect Scale if True</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###mnsNodeRelationshipNode
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mnsNodeRelationshipNode(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: nodeRelationship] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
<li><b>master</b>(<i>str</i>) ; [default: None]</li>
<li><b>slaves</b>(<i>list</i>) ; [default: [' ']]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###mnsPointsOnCurveNode
<font color = #5f5f5f size = 3pt>
<i>
Creates an mnsPointOnCurve node based on specified parameters and outputs. <br>
A 'buildOutputs' parameter is defaulted to True to build output (of a choice of any mnsType). <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mnsPointsOnCurveNode(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict ('node': MnsNameStd, 'samplesSTDs': output MnsNameStd list, 'samples': output node list)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: pointsOnCurve] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
<li><b>inputCurve</b>(<i>str</i>) - name of the curve object to connect as input curve into the node. Setting as nothing or an invalid name will result in nothing connected</li>
<li><b>inputUpCurve</b>(<i>str</i>) - name of the up-curve object to connect as input up-curve into the node. Setting as nothing or an invalid name will result in nothing connected</li>
<li><b>transforms</b>(<i>list</i>) ; [default: [' ']] - array of object to output to</li>
<li><b>buildMode</b>(<i>int</i>) - Node's build mode attribute</li>
<li><b>numOutputs</b>(<i>int</i>) ; [default: 10] - set the number of outputs or samples to be outputed from the node</li>
<li><b>doRoatate</b>(<i>bool</i>) ; [default: True] - Node's 'doRotate' attribute</li>
<li><b>rotateMode</b>(<i>int</i>) - Node's 'rotateMode' attribute</li>
<li><b>upMode</b>(<i>int</i>) ; [default: 1] - Node's 'upMode' attribute</li>
<li><b>aimAxis</b>(<i>int</i>) - Node's 'aimAxis' attribute</li>
<li><b>upAxis</b>(<i>int</i>) ; [default: 1] - Node's 'upAxis' attribute</li>
<li><b>doScale</b>(<i>bool</i>) ; [default: True] - Node's 'doScale' attribute</li>
<li><b>doSpring</b>(<i>bool</i>) - Node's 'doSpring' attribute</li>
<li><b>connectTranslate</b>(<i>bool</i>) ; [default: True] - Translate connect to the outputs if True</li>
<li><b>connectRotate</b>(<i>bool</i>) ; [default: True] - Rotate connect to the outputs if True</li>
<li><b>connectScale</b>(<i>bool</i>) ; [default: True] - Scale connect to the outputs if True</li>
<li><b>buildOutputs</b>(<i>bool</i>) ; [default: True] - in case output array is empty or invalid, build outpus as outputbuildType and outputBuildName</li>
<li><b>outputBuildSuffix</b>(<i>str</i>) ; [default: OutSample] - suffix fom built outputs, if chosen to build</li>
<li><b>buildType</b>(<i>int</i>) - if buildOutputs is executing, build based on this type.</li>
<li><b>buildVisGeo</b>(<i>bool</i>) - build axisVisGeo for the samples (debug mode)</li>
<li><b>buildVisCubes</b>(<i>bool</i>) - build axisVisGeo for the samples (debug mode)</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###reverseNode
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>reverseNode(inputA = None, output = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>inputA</b>(<i>str</i>) ; [default: None]</li>
<li><b>output</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: reverse] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###setAttrAttempt
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setAttrAttempt(nodeAttr, value, valType)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>nodeAttr</b></li>
<li><b>value</b></li>
<li><b>valType</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>