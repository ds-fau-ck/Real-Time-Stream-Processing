
### **Project Overview: Real-Time Stream Processing with Azure Event Hub**

In this project, an Azure Event Hub namespace is created to handle real-time data streams. Within the Event Hub namespace, two Event Hubs (similar to topics in message brokers) are set up, named **"bookings"** and **"payments"**, to receive continuous streams of data.
![eventbooking!](eventbooking.png)

The objective is to listen to these two data streams and perform real-time join operations using a **tumbling window**, enabling the correlation of booking and payment data as it is generated. After the join operation, the resulting data is then inserted into **Azure Synapse Analytics** for storage and further analysis.


The main tasks of the project are as follows:

1. **Publish Mock Data**: Simulate and publish mock data from the python scripts to the **bookings** and **payments** Event Hubs.
2. **Real-Time Data Transformation and Join Operations**: Use an **Azure Stream Analytics Job** to listen to both streams, apply real-time data transformation, and perform window-based join operations using a **tumbling window**.
3. **Query and Data Insertion**: Write the necessary query to implement the transformations and join operations, and then insert the final joined data into a **Synapse Analytics** table for storage and analysis.

