## Software Installation

The best way to run the course software is to use a **Docker container**. There’s full documentation on installing Docker at ``docker.com``, but in a few words, the steps are:

+ Go to ``docs.docker.com`` in your browser.
+ Step one of the instructions sends you to download Docker.
+ Run that downloaded file to install Docker.
+ At the end of the install process a whale in the top status bar indicates that Docker is running, and accessible from a terminal.
+ Click the whale to get ``Preferences``, and other options.
+ Open a command-line terminal, and run some Docker commands to verify that Docker is working as expected.
Some good commands to try are ``docker version`` to check that you have the latest release installed, and ``docker ps`` and ``docker run hello-world`` to verify that Docker is running. 
+ By default, Docker is set to use 2 processors. You can increase processing power for the app by setting this to a higher number in ``Preferences``, or lower it to have Docker for Mac use fewer computing resources.
+ Memory - By default, Docker is set to use 2 GB runtime memory, allocated from the total available memory on your computer. You can increase the RAM on the app to get faster performance by setting this number higher (for example to 3) or lower (to 1) if you want Docker to use less memory.

Once Docker is installed, you can dowload the image of this course and dowload the git repository:

+ In a terminal, go to your course folder and run (This operation requires a good internet connection; it will take some minutes):  ``docker pull shugert/deeplearning``    
+ MacOS & Linux: Run the ``shugert/deeplearning`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v /$(pwd):/notebooks shugert/deeplearning``
+ Windows: Run the ``shugert/deeplearning`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v C:/your/course/folder:/notebooks shugert/deeplearning``
+ Once these steps have been done, you can check the installation by starting your web browser and introducing this  URL: ``http://localhost:8888``.

Next times, you can bring your local copy of the repository up to date:

+ Windows: In a terminal, go to your course folder and run the ``shugert/deeplearning`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v C:/your/course/folder:/notebooks shugert/deeplearning``.
+ MacOS & Linux: In a terminal, go to your course folder and run the ``shugert/deeplearning`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v /$(pwd):/notebooks shugert/deeplearning``
+ Start your web browser and introduce this  URL: ``http://localhost:8888``.
