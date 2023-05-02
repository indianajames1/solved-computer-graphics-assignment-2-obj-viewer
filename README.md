Download Link: https://assignmentchef.com/product/solved-computer-graphics-assignment-2-obj-viewer
<br>



<ul>

 <li>Only accept answers submitted via git push to this course project for you at <a href="https://hconnect.hanyang.ac.kr/">https://hconnect.hanyang.ac.kr</a> (&lt;Year&gt;_&lt;Course no.&gt;_&lt;Class code&gt;/&lt;Year&gt;_&lt;Course</li>

</ul>

no.&gt;_&lt;Student ID&gt;.git).

<ul>

 <li>Place your files under the directory structure <strong>&lt;Assignment name&gt;/&lt;your files&gt;</strong> just like</li>

</ul>

the following example.

<table width="234">

 <tbody>

  <tr>

   <td width="234">+ 2020_ITE0000_2019000001+ ClassAssignment1/–  main.py–  report.docx</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>The submission time is determined not when the commit is made but when the git push</li>

</ul>

is made.




<ol>

 <li>Implement your own obj file viewer. The loaded mesh should be rendered with multiple light sources.

  <ol>

   <li>You have to implement all requirements in a single program. This assignment DOES NOT require each requirement to be a separate program</li>

   <li>The window size doesn’t need to be (480, 480). Use the larger window that is enough to</li>

  </ol></li>

</ol>

see the details of the viewer.




<ol start="2">

 <li><strong>Requirements </strong></li>

 <li><strong> Manipulate the camera in the same way as in ClassAssignment1 using your </strong></li>

</ol>

<strong>ClassAssignment1 code (10 pts). </strong>

<ol>

 <li>Also draw the reference grid plane.</li>

</ol>




<ol>

 <li><strong> Load an obj file and render it (70 pts) </strong>

  <ol>

   <li>Open an obj file by drag-and-drop to your obj viewer window <strong>(10 pts)</strong>

    <ol>

     <li>Google glfwSetDropCallback to see how to do it</li>

     <li>The viewer should render only one obj file at a time. If an obj file B is drag-anddropped to the viewer while it is rendering another obj file A, the viewer should</li>

    </ol></li>

  </ol></li>

</ol>

only render the new obj file B.

<ol start="3">

 <li><strong>This feature is essential for scoring your assignment, so if not implemented, </strong></li>

</ol>

<strong>you won’t get any score for “Load an obj file and render it (70 pts)” </strong>

<ol>

 <li>Read the obj file and display the mesh only using vertex positions, vertex normals, faces information <strong>(40 pts)</strong>

  <ol>

   <li>Ignore texture coordinate, material, group, shading information. In other words,</li>

  </ol></li>

</ol>

ignore vt, mtllib, usemtl, o, s tags.

<ol start="2">

 <li>Use glDrawArrays() or glDrawElements() to render triangle meshes.</li>

 <li><strong>DO NOT use glVertex*() &amp; glNormal*()</strong>. If you draw meshes using glVertex*()</li>

</ol>

&amp; glNormal*(), you’ll get only 10 pts out of 40 pts.

<ul>

 <li>Toggle wireframe / solid mode by pressing <strong>Z key</strong> (similar to pressing Z key in Blender)</li>

</ul>

<strong>(10 pts)</strong>

<ol>

 <li>When open an obj file, print out the following information of the obj file to stdout (console) <strong>(10 pts)</strong>

  <ol>

   <li>File name</li>

   <li>Total number of faces</li>

   <li>Number of faces with 3 vertices</li>

   <li>Number of faces with 4 vertices</li>

   <li>Number of faces with more than 4 vertices</li>

  </ol></li>

</ol>




<ol>

 <li><strong> Lighting (10 pts) </strong></li>

</ol>

<ol>

 <li>Use multiple light sources (not a single light) to better visualize the mesh<strong> (10 pts)</strong></li>

 <li>Choose the number of light sources, light source types, light colors, material colors as you want.</li>

</ol>




<ol start="3">

 <li><strong>Report (10 pts) </strong>

  <ol>

   <li>Submit a report of <strong>at most 2 pages</strong> in docx file format (MS Word). Do not exceed the</li>

  </ol></li>

</ol>

limit.

<ol>

 <li>The report should include:

  <ol>

   <li>Which requirements you implemented (5 pts) ii.A few screenshot images of your program with downloaded obj files (5pts)

    <ol>

     <li>Download cool obj files from the Internet and open them with your viewer. You may download obj files from

      <ol>

       <li><a href="https://free3d.com/">https://free3d.com/</a></li>

       <li><a href="https://www.cgtrader.com/free-3d-models">https://www.cgtrader.com/free</a><a href="https://www.cgtrader.com/free-3d-models">–</a><a href="https://www.cgtrader.com/free-3d-models">3d</a><a href="https://www.cgtrader.com/free-3d-models">–</a><a href="https://www.cgtrader.com/free-3d-models">models</a></li>

      </ol></li>

     <li>Choose some of the best looking screenshot images of your viewer.</li>

     <li>Do not use the sample obj files for this requirement. You must use other obj files</li>

    </ol></li>

  </ol></li>

</ol>

downloaded from internet to get score for this requirement.

iii.       Lighting configuration:

<ol>

 <li>How many light sources?</li>

 <li>Where do you put the light sources?</li>

 <li>What is the type of each light source (point light or directional light)?</li>

</ol>

<ol>

 <li>You do not need to try to write a long report. Just write down the required information.</li>

</ol>

Use either English or Korean.




<ol start="4">

 <li><strong>Extra credits </strong>

  <ol>

   <li>Toggle [shading using normal data in obj file] / [forced smooth shading] by pressing <strong>S key </strong></li>

  </ol></li>

</ol>

<strong>(+10 pts)</strong>

<ol>

 <li>In [forced smooth shading] mode, do not use vertex normal in obj. Instead, you have to compute the averaged vertex normal for each vertex as described in the lecture</li>

</ol>

slide and use them for shading.

<ol>

 <li>Load &amp; render a mesh that does not have the same number of vertices of all polygons using glDrawArrays() or glDrawElements() <strong>(+10 pts)</strong>

  <ol>

   <li>For example, some polygons in the mesh are triangles and the rest are quads or</li>

  </ol></li>

</ol>

polygons with more vertices

<ol>

 <li>To render this kind of mesh using a vertex array, you might need to render a quad or a n-polygon as a set of triangles. So you may need some kind of “triangulation”</li>

</ol>

algorithm.




<ol start="5">

 <li><strong>Runtime Environment </strong>

  <ol start="3">

   <li><strong>Your program should be able to run on systems only with Python 3.7 or later, NumPy, </strong></li>

  </ol></li>

</ol>

<strong>PyOpenGL, glfw. Do not use any other additional python modules. </strong>

<ol>

 <li>Only <strong>glfw</strong> is allowed for event processing and window &amp; OpenGL context management. <strong>Do not use glut functions for this purpose.</strong></li>

 <li><strong>If your program does not meet this requirement, it will not run on TA’s computer </strong><strong>so </strong></li>

</ol>

<strong>you will not get any score for this assignment (except report). </strong>

<strong> </strong>

<ol start="6">

 <li><strong>Test your viewer with sample obj files. </strong> cube-tri.obj: A cube with triangles only

  <ol>

   <li>cube-tri-quad.obj: A cube with triangles and quads</li>

   <li>sphere-tri.obj: A sphere with triangles only</li>

   <li>sphere-tri-quad.obj: A sphere with triangles and quads</li>

   <li>cylinder-tri.obj: A cylinder with triangles only</li>

   <li>cylinder-tri-quad-n.obj: A cylinder with triangles, quads and polygons with more vertices</li>

   <li><strong>Basically, your viewer should be able to render cube-tri.obj, sphere-tri.obj, cylinder-</strong></li>

  </ol></li>

</ol>

<strong>tri.obj properly. </strong>

<ol>

 <li><strong>To meet extra credit requirement B, your viewer should be able to render all above </strong></li>

</ol>

<strong>sample obj files properly. </strong>




<ol start="7">

 <li><strong>What you have to submit: </strong>

  <ol>

   <li><strong>.py files</strong>

    <ol>

     <li>You can use multiple .py files for this assignment. In this case, explain how to run the</li>

    </ol></li>

  </ol></li>

</ol>

program in the report.

<ol>

 <li><strong>.docx report file</strong></li>

</ol>




<ol start="8">

 <li>Additional information

  <ol>

   <li>drop_callback in glfw python binding is slightly different from that of original glfw written in C. drop_callback in python takes only two parameters, window and paths. paths is a list</li>

  </ol></li>

</ol>

of dropped file paths.

<ol>

 <li>obj file format reference: <a href="https://en.wikipedia.org/wiki/Wavefront_.obj_file">https://en.wikipedia.org/wiki/Wavefront_.obj_file</a></li>

 <li>Python provides powerful string methods helpful for parsing an obj file. Among them, split() will be most useful.</li>

</ol>