# cse4020-lab-8-solved
**TO GET THIS SOLUTION VISIT:** [CSE4020 Lab 8 Solved](https://www.ankitcodinghub.com/product/cse4020-lab-8-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91696&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE4020 Lab 8 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
1. Write down a Python program to draw a transformed triangle in a 3D space.

<ol>
<li>Set the window title to your student ID and the window size to (480,480).</li>
<li>Use the following code snippet:</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="section">
<div class="layoutArea">
<div class="column">
gCamAng = 0

</div>
</div>
<div class="layoutArea">
<div class="column">
gComposedM = np.identity(4)

</div>
</div>
<div class="layoutArea">
<div class="column">
def render(M, camAng):

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre># enable depth test
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
glClear(GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT)

</div>
</div>
<div class="layoutArea">
<div class="column">
glEnable(GL_DEPTH_TEST)

</div>
</div>
<div class="layoutArea">
<div class="column">
glLoadIdentity()

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre># use orthogonal projection
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
glOrtho(-1,1, -1,1, -1,1)

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre># rotate "camera" position to see this 3D space better
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
gluLookAt(.1*np.sin(camAng),.1, .1*np.cos(camAng), 0,0,0, 0,1,0)

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre># draw coordinate: x in red, y in green, z in blue
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
glBegin(GL_LINES)

</div>
</div>
<div class="layoutArea">
<div class="column">
glColor3ub(255, 0, 0)

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv(np.array([0.,0.,0.])) glVertex3fv(np.array([1.,0.,0.]))

</div>
</div>
<div class="layoutArea">
<div class="column">
glColor3ub(0, 255, 0)

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv(np.array([0.,0.,0.])) glVertex3fv(np.array([0.,1.,0.]))

</div>
</div>
<div class="layoutArea">
<div class="column">
glColor3ub(0, 0, 255)

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv(np.array([0.,0.,0]))

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv(np.array([0.,0.,1.]))

</div>
</div>
<div class="layoutArea">
<div class="column">
glEnd()

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre># draw triangle
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
glBegin(GL_TRIANGLES)

</div>
</div>
<div class="layoutArea">
<div class="column">
glColor3ub(255, 255, 255)

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv((M @ np.array([.0,.5,0.,1.]))[:-1]) glVertex3fv((M @ np.array([.0,.0,0.,1.]))[:-1]) glVertex3fv((M @ np.array([.5,.0,0.,1.]))[:-1])

</div>
</div>
<div class="layoutArea">
<div class="column">
glEnd()

</div>
</div>
<div class="layoutArea">
<div class="column">
def key_callback(window, key, scancode, action, mods):

</div>
</div>
<div class="layoutArea">
<div class="column">
global gCamAng, gComposedM

</div>
</div>
<div class="layoutArea">
<div class="column">
if action==glfw.PRESS or action==glfw.REPEAT:

</div>
</div>
<div class="layoutArea">
<div class="column">
if key==glfw.KEY_1:

</div>
</div>
<div class="layoutArea">
<div class="column">
gCamAng += np.radians(-10)

</div>
</div>
<div class="layoutArea">
<div class="column">
elif key==glfw.KEY_3:

</div>
</div>
<div class="layoutArea">
<div class="column">
gCamAng += np.radians(10)

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
C. If you press or repeat a key, the triangle should be transformed as shown in the Table. Note that key 1 and 3 are already implemented in the above code snippet.

Key

Q

E Translate by 0.1 in x direction w.r.t global coordinate

A Rotate about y axis by -10 degrees w.r.t local coordinate

D Rotate about y axis by +10 degrees w.r.t local coordinate W Rotate about x axis by -10 degrees w.r.t local coordinate S Rotate about x axis by +10 degrees w.r.t local coordinate

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Transformation

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Translate by -0.1 in x direction w.r.t global coordinate

</div>
</div>
</td>
</tr>
</tbody>
</table>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
1 Rotate camera -10 degree

3 Rotate camera 10 degree

D. Transformations should be accumulated (composed with previous one).

E. Files to submit: A Python source file (Name the file whatever you want (in English). Extension should be .py)

2. Write down a Python program to draw a hierarchical model of boxes.

<ol>
<li>Set the window title to your student ID and the window size to (480,480).</li>
<li>Start from the following code skeleton.</li>
</ol>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
import glfw

</div>
</div>
<div class="layoutArea">
<div class="column">
from OpenGL.GL import *

</div>
</div>
<div class="layoutArea">
<div class="column">
import numpy as np

</div>
</div>
<div class="layoutArea">
<div class="column">
from OpenGL.GLU import *

</div>
</div>
<div class="layoutArea">
<div class="column">
def render():

</div>
</div>
<div class="layoutArea">
<div class="column">
glClear(GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT)

</div>
</div>
<div class="layoutArea">
<div class="column">
glEnable(GL_DEPTH_TEST)

</div>
</div>
<div class="layoutArea">
<div class="column">
glMatrixMode(GL_PROJECTION)

</div>
</div>
<div class="layoutArea">
<div class="column">
glLoadIdentity()

</div>
</div>
<div class="layoutArea">
<div class="column">
glOrtho(-2,2, -2,2, -1,1)

</div>
</div>
<div class="layoutArea">
<div class="column">
glMatrixMode(GL_MODELVIEW)

</div>
</div>
<div class="layoutArea">
<div class="column">
glLoadIdentity()

</div>
</div>
<div class="layoutArea">
<div class="column">
drawFrame()

</div>
</div>
<div class="layoutArea">
<div class="column">
t = glfw.get_time()

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre># blue base transformation
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
glPushMatrix()

</div>
</div>
<div class="layoutArea">
<div class="column">
glTranslatef(np.sin(t), 0, 0)

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre># blue base drawing
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
glPushMatrix()

</div>
</div>
<div class="layoutArea">
<div class="column">
glScalef(.2, .2, .2)

</div>
</div>
<div class="layoutArea">
<div class="column">
glColor3ub(0, 0, 255)

</div>
</div>
<div class="layoutArea">
<div class="column">
drawBox()

</div>
</div>
<div class="layoutArea">
<div class="column">
glPopMatrix()

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre># red arm transformation
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
glPushMatrix()

</div>
</div>
<div class="layoutArea">
<div class="column">
glRotatef(t*(180/np.pi), 0, 0, 1)

</div>
</div>
<div class="layoutArea">
<div class="column">
glTranslatef(.5, 0, .01)

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre># red arm drawing
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
glPushMatrix()

</div>
</div>
<div class="layoutArea">
<div class="column">
glScalef(.5, .1, .1)

</div>
</div>
<div class="layoutArea">
<div class="column">
glColor3ub(255, 0, 0)

</div>
</div>
<div class="layoutArea">
<div class="column">
drawBox()

</div>
</div>
<div class="layoutArea">
<div class="column">
glPopMatrix()

</div>
</div>
<div class="layoutArea">
<div class="column">
glPopMatrix() glPopMatrix()

</div>
</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="section">
<div class="layoutArea">
<div class="column">
def drawBox():

</div>
</div>
<div class="layoutArea">
<div class="column">
glBegin(GL_QUADS)

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv(np.array([1,1,0.]))

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv(np.array([-1,1,0.]))

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv(np.array([-1,-1,0.]))

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv(np.array([1,-1,0.]))

</div>
</div>
<div class="layoutArea">
<div class="column">
glEnd()

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
def drawFrame():

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre># draw coordinate: x in red, y in green, z in blue
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
glBegin(GL_LINES)

</div>
</div>
<div class="layoutArea">
<div class="column">
glColor3ub(255, 0, 0)

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv(np.array([0.,0.,0.])) glVertex3fv(np.array([1.,0.,0.]))

</div>
</div>
<div class="layoutArea">
<div class="column">
glColor3ub(0, 255, 0)

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv(np.array([0.,0.,0.])) glVertex3fv(np.array([0.,1.,0.]))

</div>
</div>
<div class="layoutArea">
<div class="column">
glColor3ub(0, 0, 255)

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv(np.array([0.,0.,0]))

</div>
</div>
<div class="layoutArea">
<div class="column">
glVertex3fv(np.array([0.,0.,1.]))

</div>
</div>
<div class="layoutArea">
<div class="column">
glEnd()

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
def main():

</div>
</div>
<div class="layoutArea">
<div class="column">
if not glfw.init():

</div>
</div>
<div class="layoutArea">
<div class="column">
return

</div>
</div>
<div class="layoutArea">
<div class="column">
window = glfw.create_window(480,480,’2017123456-lab6-1′, None,None)

</div>
</div>
<div class="layoutArea">
<div class="column">
if not window:

</div>
</div>
<div class="layoutArea">
<div class="column">
glfw.terminate()

</div>
</div>
<div class="layoutArea">
<div class="column">
return

</div>
</div>
<div class="layoutArea">
<div class="column">
glfw.make_context_current(window)

</div>
</div>
<div class="layoutArea">
<div class="column">
glfw.swap_interval(1)

</div>
</div>
<div class="layoutArea">
<div class="column">
while not glfw.window_should_close(window):

</div>
</div>
<div class="layoutArea">
<div class="column">
glfw.poll_events()

</div>
</div>
<div class="layoutArea">
<div class="column">
render()

</div>
</div>
<div class="layoutArea">
<div class="column">
glfw.swap_buffers(window)

</div>
</div>
<div class="layoutArea">
<div class="column">
glfw.terminate()

</div>
</div>
<div class="layoutArea">
<div class="column">
if __name__ == “__main__”:

</div>
</div>
<div class="layoutArea">
<div class="column">
main()

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
C.

D.

E.

</div>
<div class="column">
Add a green arm at the end of the red arm, and rotate the green arm about its local z axis.

i. Render the green arm using drawBox().

Also render local frames of the blue base, red arm, green arm using drawFrame().

Expected result: Uploaded LabAssignment8-2.mp4

</div>
</div>
<div class="layoutArea">
<div class="column">
F. Files to submit: A Python source file (Name the file whatever you want (in English). Extension should be .py)

</div>
</div>
</div>
