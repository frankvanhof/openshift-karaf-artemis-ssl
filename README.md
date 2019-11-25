# Camel AMQ QuickStart

This quickstart demonstrates how to connect to an Artemis broker on OpenShift and use JMS messaging between two Camel routes.


### Configuration

Before running the quickstart, you need to configure the `src/main/fabric8/deployment.yml` file in order to 
use the correct remote instance of the Artemis Broker.

### Building

The example can be built with:

    mvn clean install

### Running the example in OpenShift

The example can be built and deployed using:

    mvn fabric8:deploy

When the example runs in OpenShift, you can use the OpenShift client tool to inspect the status, e.g.:

- To list all the running pods:
    ```
    $ oc get pods
    ```

- Then find the name of the pod that runs this example, and output the logs from the running pod with:
    ```
    $ oc logs <name of pod>
    ```
