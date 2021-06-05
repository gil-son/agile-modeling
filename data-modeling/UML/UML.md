## UML Class Relationships

### Introduction

<p>
	 UML diagrams are the abstract way of looking at things, regardless of their size, whether real or virtual. 
	In Object Orientation, the class can be represented by diagrams. A Class can be related to other classes, 
	relate to itself or just not relate.
</p>


<div align="center">
	
![image](https://d3n817fwly711g.cloudfront.net/uploads/2012/03/Class-Diagram-Relationships.png)
	
</div>

### Parts of Class Diagrams

The following figure is an example of a simples class:

<div align="center">
	
![image](https://d3n817fwly711g.cloudfront.net/blog/wp-content/uploads/2012/03/Class-Diagram.jpeg)
	
</div>

<p>
In the example, a class called “loan account” is depicted. Classes in class diagrams are represented by boxes that are partitioned into three:	
</p>


<ol>
  <li> The top partition contains the name of the class</li>
  <li> The middle part contains the class’s attributes</li>
  <li> The bottom partition shows the possible operations that are associated with the class</li>
</ol>

### Comuns Annotations

<table>
    <tr>
       <th>Type</th>
       <th>Signific</th>
     </tr>
     <tr>
        <td>0..1</td>
        <td>Zero or one instance</td>
     </tr>
     <tr>
        <td>0..* or *</td>
        <td>Zero or n instance</td>
     </tr>
     <tr>
        <td>1</td>
        <td>One instance</td>
     </tr>
     <tr>
        <td>1..*</td>
        <td>One or n instance</td>
     </tr>
</table>



### Relationships in Class Diagrams

<p> Classes are interrelated to each other in specific ways. In particular, relationships in class diagrams include different types of logical connections. The following are such types of logical connections that are possible in UML:
</p>



<ul>
  <li><a href="#"></a>Association</li>
  <li><a href="#"></a>Directed Association</li>
  <li><a href="#"></a>Reflexive Association</li>
  <li><a href="#"></a>Multiplicity</li>
  <li><a href="#"></a>Aggregation</li>
  <li><a href="#"></a>Composition</li>
  <li><a href="#"></a>Inheritance/Generalization</li>
  <li><a href="#"></a>Realization</li>
</ul>


## Association

<div align="center">
	
![image](https://d3n817fwly711g.cloudfront.net/blog/wp-content/uploads/2012/03/Association-Relationship.jpeg)
	
</div>

<p>is a broad term that encompasses just about any <b>logical connection</b> or <b>relationship between classes</b>. For example, passenger and airline may be linked as above:</p>


## Directed Association:

<div align="center">
	
![image](https://d3n817fwly711g.cloudfront.net/blog/wp-content/uploads/2012/03/Directed-Association-Relationship.jpeg)
	
</div>	
	
<p>refers to a directional relationship represented by a <b>line with an arrowhead</b>. The arrowhead depicts a container-contained directional flow.</p>

	
## Reflexive Association

<div align="center">
	
![image](https://d3n817fwly711g.cloudfront.net/blog/wp-content/uploads/2012/03/Reflexive-Association-Relationship.jpeg)
	
</div>

<p> This occurs when a class <b>may have multiple functions</b> or <b>responsibilities</b>. For example, a staff member working in an airport may be a pilot, aviation engineer, a ticket dispatcher, a guard, or a maintenance crew member. If the maintenance crew member is managed by the aviation engineer there could be a managed by relationship in two instances of the same class.</p>
</div>
	
## Multiplicity
	
<div align="center">
	
![image](https://d3n817fwly711g.cloudfront.net/blog/wp-content/uploads/2012/03/Multiplicity-Relationship.jpeg)
	
</div>

<p>is the active logical association when the <b>cardinality of a class in relation to another is being depicted</b>. For example, one fleet may include multiple airplanes, while one commercial airplane may contain zero to many passengers. The notation 0..* in the diagram means “zero to many”.</p>

### Aggregation

<div align="center">
	
![image](https://d3n817fwly711g.cloudfront.net/blog/wp-content/uploads/2012/03/Aggregation-Relationship.png)
	
</div>

<p>refers to the formation of a particular <b>class as a result of one class being aggregated</b> or <b>built as a collection</b>. For example, the class “library” is made up of one or more books, among other materials. In aggregation, the contained classes are not strongly dependent on the lifecycle of the container. In the same example, books will remain so even when the library is dissolved.</p>

<p>To show aggregation in a diagram, draw a line from the parent class to the child class with a diamond shape near the parent class.</p>

### Composition

<div align="center">
	
![image](https://d3n817fwly711g.cloudfront.net/blog/wp-content/uploads/2012/03/Composition-Relationship-UML.png)
	
</div>

<p> The composition relationship is very <b>similar to the aggregation relationship</b>. with the <b>only difference being its key purpose of emphasizing the dependence of the contained class to the life cycle of the container class</b>. That is, the contained class will be obliterated when the container class is destroyed. For example, a shoulder bag’s side pocket will also cease to exist once the shoulder bag is destroyed.</p>

<p> To show a composition relationship in a UML diagram, <b>use a directional line connecting the two classes</b>, with <b>a filled diamond shape adjacent to the container class and the directional arrow to the contained class</b>.</p>

### Inheritance
<div align="center">
	
![image](https://d3n817fwly711g.cloudfront.net/blog/wp-content/uploads/2012/03/Inheritance-Relationship.jpeg)
	
</div>

<p>refers to a type of <b>relationship wherein one associated class is a child of another by virtue of assuming the same functionalities of the parent class</b>. In other words, the child class is a specific type of the parent class.</p>

<p> To show inheritance in a UML diagram, a solid line from the child class to the parent class is drawn using an unfilled arrowhead.</p>

### Realization

<div align="center">
	
![image](https://user-images.githubusercontent.com/72712095/120896032-07e4e480-c5f6-11eb-847c-c8cb04138615.png)
	
</div>

<p>denotes the <b>implementation of the functionality defined in one class by another class</b>. To show the relationship in UML, a broken line with an unfilled solid arrowhead is drawn from the class that defines the functionality of the class that implements the function. In the example, the printing preferences that are set using the printer setup interface are being implemented by the printer.</p>


### Sources

<ul>
	
   <li><a href="https://developer.ibm.com/articles/the-class-diagram/">IBM - Articles - The class diagram</a></li>
  <li><a href="https://creately.com/blog/diagrams/class-diagram-relationships/">Creately</a></li>
  <li><a href="http://www.dsc.ufcg.edu.br/~jacques/cursos/map/html/uml/diagramas/classes/classes3.htm">DSC - UFCG</a></li>
</ul>

