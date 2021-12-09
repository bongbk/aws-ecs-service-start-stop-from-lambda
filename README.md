1. you need to create a Lambda function and add this Python script
2. The script expects the following variables in a JSON format:
{
  "cluster": "clusterName",
  "service_names": "service1,service2",
  "service_desired_count": "0"
}
Where:

cluster is the name of the cluster you want to modify.
service_names is an array for the collection of services.
service_desired_count is the number of desired services. 0 is to stop the service/s, any other number is to start the service/s.

3. Go to CloudWatch Events to create schedule and paste script to Constant (JSON text)
