# robo

Basic idea

A robotic brain that uses containers as neural nodes for processing robotic operations. The initial stage of this will be to use a library such as gocv to build out the visual processing services of the robotic framework. My idea is that each microservice would act as either serverless functions, or as individual subscribers to data being recieved from the capture device. As the data is processed by the individual microservices the resulting identifications and tracking that results is then passed to a processing unit for storage and further use. 

The docker containers for the individual services can be either on the device itself or in the cloud. 

While the visual nodes will provide necessary processing capability for handling data recieved from a camera or images, this doesn't provide what to do with that data after it is received. The next step as I see it would be to add in a neural network that handles what to do with that image data as well as other sensor data. This can range from designating it for storage, identifying commands to send to attached devices (motors, speakers, communication, etc...)