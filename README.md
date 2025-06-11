# cs3241-lab-2-solved
**TO GET THIS SOLUTION VISIT:** [CS3241 Lab 2 Solved](https://mantutor.com/product/cs3241-solved-10/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;113004&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS3241 Lab 2  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 138px;">
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
            5/5 - (3 votes)    </div>
    </div>
LEARNING OBJECTIVES

OpenGL viewing, OpenGL transformations, hierarchical modeling, and animation. After completing the programming assignment, you should have learned

• how to set up the view transformation (camera position and orientation) in OpenGL,

• how to set up perspective viewing in OpenGL,

• how to use the OpenGL transformations for modeling, and • how to use the OpenGL transformations for animation.

TASKS

From the Canvas &gt; CS3241 &gt; Files &gt; Lab Assignments folder, download the ZIP file Lab2_todo_(*).zip.

You are provided with an incomplete C++ application program main.cpp, and your job is to complete it according to the requirements.

+x main_done to give the file execute permission before running it.)

Please read the instructions shown in the console/terminal window to learn how to operate the program. When you run the program, you should see a spherical planet at the center of the window.

There are a dozen cars moving on the planet surface, and each car moves in a different great circle (you can search the web to find out what a great circle is), and they have different speeds and colors.

• resize the window and see what happens,

• press the Up, Down, Left or Right arrow key to change the camera’s position, • press the Page Up or Page Down key to change the camera’s distance from the planet,

• press the ‘P’ key to pause/resume the animation of the cars.

You will notice that the camera is always looking at the center of the planet. With respect to the planet, the camera’s position can be expressed as latitude and longitude, and its distance from the planet’s center. When the Left or Right arrow key is pressed, the camera’s longitude decreases or increases, respectively; and when the Down or Up arrow key is pressed, the camera’s latitude decreases or increases, respectively. Note that the camera’s up-vector is always pointing north.

Figure 1

Follow the following instructions to complete main.cpp as required. You must not add or change any other files.

1) Study the source program very carefully.

2) Complete the DrawOneCar() function. The function must draw the car using only GLUT functions such as glutSolidCube(), glutSolidTorus(), glutSolidCone(), and glutSolidSphere(). You should not directly use any OpenGL geometric primitive. You should make use of the OpenGL 3D transformation functions to help you resize, orientate and position the parts. The functions glPushMatrix() and glPopMatrix() are very helpful for you to save and restore the current transformation before and after drawing each part. You can design your cars any way you like as long as they look like cars. More details about the GLUT functions can be found at https://www.opengl.org/resources/libraries/glut/spec3/spec3.html.

3) Complete the DrawAllCars() function. This function draws each car at the correct position on its great circle. Note that any great circle on a sphere centered at the origin can be defined as follows. Let C be the great circle in the y = 0 plane, and let v be a vector in the x-z plane, and let  be an angle. If we rotate C about v by , we get another great circle of the sphere. All great circles of the sphere can be obtained by varying v and .

4) Set up the correct perspective viewing volume in the MyDisplay() function. You should use the gluPerspective() function. The near and far planes should be set near the planet’s surface, yet still do not clip off any part of the planet and cars. The near and far planes should vary with the eye’s distance from the planet’s center. You should make use of the value of the predefined constant CLIP_PLANE_DIST to position your near and far planes.

6) Complete the MyTimer() function. You should use the GLUT timer callback to control the speed of the animation by maintaining a constant frame rate (DESIRED_FPS). Refer to https://www.opengl.org/resources/libraries/glut/spec3/node64.html to find out more about the GLUT function glutTimerFunc().

DO NOT HARD-CODE VALUES. You should write your code in such a way that when the values of the named constants (defined in the beginning of the program) are changed to other valid values, your program should function accordingly. For example, if the car’s size is changed, the tyre size should vary proportionally.

GRADING

Good coding style. Comment your code adequately, use meaningful names for functions and variables, and indent your code properly. You must fill in your name, and NUS User ID in the header comment.

SUBMISSION

For this assignment, you need to submit only your completed main.cpp.

You must put it/them in a ZIP file and name your ZIP file nus-user-id_lab2.zip. For example, if your NUS User ID is e0123456, you should name your file e0123456_lab2.zip.

Note that you will be penalized for submitting non-required files.

——— End of Document ———
