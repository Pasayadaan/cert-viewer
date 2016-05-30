Digital Certificates Viewer Project
===================================

Flask webapp to display and verify digital certificates after they have been issued and to allow learners to
 request a certificate and generate their own Bitcoin identity needed for the certificate creation process. [See the schema](https://github.com/digital-certificates/schema>)

Documentation
-------------

[http://viewer.readthedocs.io/](http://viewer.readthedocs.io/)


Quick start
-----------

### Steps

1. [Install docker](https://docs.docker.com/engine/installation)
    - There's a lot of introductory information; installation steps start at the #installation anchor for your os. For
example, mac instructions start at [https://docs.docker.com/engine/installation/mac/#installation](https://docs.docker.com/engine/installation/mac/#installation)

2. Git clone the repository

    ```
    git clone https://github.com/digital-certificates/viewer.git
    ```

3. Build the container with docker-compose

    ```
    docker-compose build
    ```

4. Start the container

    ```
    docker-compose up
    ```

5. Access the certificate-viewer pre-populated with test data at `http://<hostname>:5000`, where hostname is given by

    ```
    docker-machine ip
    ```


###About Docker Setup
The quick start steps do the following:

1. Creates a container that runs the certificate-viewer Flask app with MongoDB using Docker Compose [details](http://containertutorials.com/docker-compose/flask-mongo-compose.html)
2. Seeds the MongoDB database with sample fake certificates. This data is located in the mongo-seed folder
3. Starts the container. This configuration exposes port 5000.


About the Digital Certificates project
--------------------------------------

The [MIT Media Lab Digital Certificates] is an incubation project. We're looking for feedback, contributions, and general
discussion. This is not currently intended for production release, but we are improving our approach for future releases.


Contact
-------

Contact [certs@media.mit.edu](mailto:certs@media.mit.edu) with questions


