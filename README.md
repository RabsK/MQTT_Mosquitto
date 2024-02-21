MQTT Mosquitto for CheriBSD and Ubuntu
=================

Message Queuing Telemetry Transport (MQTT) is a lightweight messaging protocol developed for efficient communication in situations with limited bandwidth, high latency, or unreliable networks. It's especially useful in Internet of Things (IoT) and Machine to Mahine (M2M) communication scenarios. MQTT operates on a publish-subscribe model, where devices, called publishers, send messages to a central message broker. Other devices, known as subscribers, can then receive these messages based on their subscriptions to specific topics.

Mosquitto, an open-source MQTT broker and client implementation maintained by the Eclipse Foundation, acts as a central hub for MQTT communication, facilitating message exchange between connected devices. Key features of Mosquitto include:

1. Publish-Subscribe Model: Mosquitto enables loosely coupled communication between devices by following the publish-subscribe messaging pattern.
2. Quality of Service (QoS) Levels: Mosquitto supports multiple QoS levels (0, 1, and 2), providing varying degrees of reliability in message delivery to meet different application needs.
3. Security Mechanisms: Mosquitto offers authentication mechanisms and encryption options such as TLS/SSL to ensure secure communication between clients and the broker.
4. Message Persistence: Mosquitto allows messages to be persisted to disk, ensuring that messages are retained even if the broker restarts, thereby enhancing reliability and durability.
5. Scalability: Designed to be lightweight and scalable, Mosquitto is suitable for deployments ranging from small-scale IoT networks to large-scale enterprise solutions.
 

## Resources

Explore the following resources for additional information about MQTT:

- Community page: <http://mqtt.org/>
- MQTT v3.1.1 standard: <https://docs.oasis-open.org/mqtt/mqtt/v3.1.1/mqtt-v3.1.1.html>
- MQTT v5.0 standard: <https://docs.oasis-open.org/mqtt/mqtt/v5.0/mqtt-v5.0.html>

Information about the Open Source  Mosquitto can be found at the following sources:
- Source code repository: <https://github.com/eclipse/mosquitto>

 ### Build Dependencies

Before getting started, it is recommended to download and install the following; 

cmake, make, xsltproc (Ubuntu), libtool, git, ninja etc.

##cJSON

If not already installed, it is recommended to install cJSON. The following steps can be used to do so;
You may use the elevated privileges if needed (sudo) or remove it if not required

    sudo git clone https://github.com/DaveGamble/cJSON.git

Change the directory to cJSON
    cd cJSON

Creat a new build directory
   
    sudo mkdir build

Change the directory to build

    cd build

Run the CMake configuration process with elevated privileges if needed

    sudo cmake ..

Execute the make command with elevated privileges if needed, you may need to use gmake instead of make if using CheirBSD
    
    sudo make

Install the compiled software components into system directories, typically requiring eevated privilages for system-wide access.

    sudo make install

And you are all set :-)


## Building the MQTT mosquitto code from source




## Credits

Mosquitto was written by Roger Light <roger@atchoo.org>
