Introduction to Problem Types
-----------------------------------------------------

Please read the following, watch the videos, and try to solve the problems.


Solving Mixed-up Code Problems
==================================

If you see a problem like the one below you will need to put the mixed-up
code in the correct order on the right side. You
may need to indent the blocks as well.  There may also be extra blocks that are not
needed in a correct solution that you can leave on the left side. Click the "Check" button
to check your solution.

See the video below for an example.

.. youtube:: Rf7oWHlo-e0
    :divid: iwgex1-parsons1-p3dnd
    :optional:
    :width: 650
    :height: 415
    :align: center

Try to solve the following mixed-up code problem.  This problem doesn't require any indentation.

.. parsonsprob:: intro-simple-parsons-no-indent-p3dnd
   :numbered: left
   :adaptive:
   :practice: T
   :order: 3, 1, 2, 0

   Drag the blocks from the left and put them in the correct order on the right. The text in each block
   defines the order.
   -----
   First block
   =====
   Second block
   =====
   Third block

Try to solve the following mixed-up code problem. This problem requires indentation.

.. parsonsprob:: intro-simple-parsons-indent-p3dnd
   :numbered: left
   :adaptive:
   :practice: T
   :order: 3, 1, 2, 0

   Drag the blocks from the left and put them in the correct order on the right with the correct indentation.
   The text in each block defines the order and indentation.
   -----
   First block
   =====
   Second block
   =====
       Third block that needs to be indented

Try to solve the following mixed-up code problem. This problem requires indentation and has extra blocks that are not needed in a correct solution.

.. parsonsprob:: intro-simple-parsons-indent-with-dist-p3dnd
   :numbered: left
   :adaptive:
   :practice: T
   :order: 3, 1, 2, 0

   Drag the blocks from the left and put them in the correct order on the right with the correct indentation.
   There is an extra block that is not needed in the correct solution.
   -----
   First block
   =====
   Second block
   =====
   Extra block that is not needed #paired: This block is not needed
   =====
       Third block that needs to be indented

The mixed-up code problems have a "Help me" button at the bottom of the
problem. Once you have checked at least three incorrect solutions you can
click the button for help.  It will remove an incorrect code block, if you used
one in your solution, or combine two blocks into one if there are more
than three blocks left.

See the video below for an example.

.. youtube:: QejZ7u642IU
    :divid: iwgex1-parsons2-p3dnd
    :optional:
    :width: 650
    :height: 415
    :align: center

Solving Write Code Problems
==============================

If you see a problem like the one below, you will need to write code.  The problem
will have unit tests that you can run to check that your code is working
correctly.  Click on the "Run" button to compile and run your code.  Look after
the code area for compiler errors and/or unit test results.

See the video below for an example.

.. youtube:: w9hTOJ7iJpE
    :divid: p3dndta-write-code-video-ex
    :optional:
    :width: 1020
    :height: 826
    :align: center

Finish writing the code for the following problem.

.. activecode:: intro-sample-write-code-triple-p3dnd
    :practice: T
    :autograde: unittest

    Write a function called ``triple(num)`` that takes a number ``num`` and
    returns the number times 3. For example, ``triple(2)`` should return 6 and
    ``triple(-1)`` should return -3.  Look below the code to check for any
    compiler errors or the results
    from the test cases.  Be sure to ``return`` the result.
    ~~~~
    def triple(num):
        # write code here

    print(triple(2))
    print(triple(-1))

    ====
    from unittest.gui import TestCaseGui
    class myTests(TestCaseGui):

        def testOne(self):
            self.assertEqual(triple(2),6,"triple(2)")
            self.assertEqual(triple(3),9,"triple(3)")
            self.assertEqual(triple(-1),-3,"triple(-1)")
            self.assertEqual(triple(0),0,"triple(0)")
            self.assertEqual(triple(11),33,"triple(11)")

    myTests().main()

Feedback
==================================

.. shortanswer:: p3dndta-intro-sa

   Please provide feedback here. Please share any comments, problems, or suggestions.


What to do next
============================

.. raw:: html

    <p>Click on the following link to go the practice problems: <a id="p3dndta-practice"><font size="+2">Practice Problems</font></a></p>


.. raw:: html

   <script type="text/javascript">

     function getCookie(cname) {
        let name = cname + "=";
        let decodedCookie = decodeURIComponent(document.cookie);
        let ca = decodedCookie.split(';');
        for(let i = 0; i <ca.length; i++) {
           let c = ca[i];
           while (c.charAt(0) == ' ') {
              c = c.substring(1);
           }
           if (c.indexOf(name) == 0) {
              return c.substring(name.length, c.length);
           }
        }
        return "";
     }

     function setCookie(cname, cvalue) {
        document.cookie = cname + "=" + cvalue + ";";
     }

     window.onload = function() {

        a = document.getElementById("p3dndta-practice")

        // get prev set cookie
        var EXP_COOKIE = 'p3dndta'
        var cond = getCookie(EXP_COOKIE);

        // if no prev set cookie: generate random condition and set cookie
        if (cond != 'd' && cond != 'nd') {
           var v = Math.floor(Math.random() * 2);
           if (v < 1) {
               cond = 'd';
           } else {
               cond = 'nd';
           }
           setCookie(EXP_COOKIE, cond);
        }

        if (cond == 'd') {
           a.href = "p3dndta-wd-nd.html"
        } else if (cond == 'nd') {
           a.href = "p3dndta-nd-wd.html"
        }
     };
   </script>
