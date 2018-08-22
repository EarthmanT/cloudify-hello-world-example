# cloudify-hello-world-example

Very simple Cloudify Hello World for AWS, Azure, GCP, and Openstack.

Only for use with a Cloudify Manager.

## Instructions

For AWS:

```shell
cfy install aws.yaml -i aws_region_name=eu-central-1
```

For Azure:

```shell
cfy install azure.yaml -i location=eastus -i agent_password=OpenS3sVm3
```

For GCP:

```shell
cfy install gcp.yaml region=europe-west1
```

For Openstack:

```shell
cfy install openstack.yaml \
    -i region=RegionOne
    -i external_network=external_network \
    -i image=05bb3a46-ca32-4032-bedd-8d7ebd5c8100 \
    -i flavor=4d798e17-3439-42e1-ad22-fb956ec22b54
```

Another Openstack example:

```shell
cfy install openstack.yaml \
     -i region=RegionOne \
     -i external_network_name=GATEWAY_NET \
     -i image=e41430f7-9131-495b-927f-e7dc4b8994c8 \
     -i flavor=2
```