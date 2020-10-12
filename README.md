# Deploy a high-availability web app using CloudFormation

<p>In this project, you’ll deploy web servers for a highly available web app using CloudFormation.</p>

Project Arcitecture:
![alt text](https://github.com/ghasemel/webapp-aws-udacity-project2/blob/master/ProjectArchitecture.png?raw=true)

In this project we deploy:
  - CloudWatch Alarms to trigger automatic scaling in/out instances. Cpu utilization of the AutoScalingGroup has been considered as the metric
  - a VPCEndpoint for connecting to the S3 bucket. In this way we can avoid data processing charges for NAT gateways. ([more info](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-gateway.html#nat-gateway-s3-ddb))
  
  
<ul>Resources:
  <li>AWS::EC2::VPC</li>
  <li>AWS::EC2::InternetGateway</li>
  <li>AWS::EC2::VPCGatewayAttachment</li>
  <li>AWS::EC2::Subnet</li>
  <li>AWS::EC2::RouteTable</li>
  <li>AWS::EC2::Route</li>
  <li>AWS::EC2::SubnetRouteTableAssociation</li>
  <li>AWS::EC2::EIP</li>
  <li>AWS::EC2::NatGateway</li>
  <li>AWS::EC2::Subnet</li>
  <li>AWS::EC2::RouteTable</li>
  <li>AWS::EC2::Route</li>
  <li>AWS::EC2::SubnetRouteTableAssociation</li>
  <li>AWS::EC2::Subnet</li>
  <li>AWS::EC2::SubnetRouteTableAssociation</li>
  <li>AWS::EC2::EIP</li>
  <li>AWS::EC2::NatGateway</li>
  <li>AWS::EC2::Subnet</li>
  <li>AWS::EC2::RouteTable</li>
  <li>AWS::EC2::Route</li>
  <li>AWS::EC2::SubnetRouteTableAssociation</li>
  <li>AWS::EC2::VPCEndpoint</li>
  <li>AWS::IAM::Role</li>
  <li>AWS::IAM::InstanceProfile</li>
  <li>AWS::EC2::SecurityGroup</li>
  <li>AWS::AutoScaling::LaunchConfiguration</li>
  <li>AWS::AutoScaling::AutoScalingGroup</li>
  <li>AWS::EC2::SecurityGroup</li>
  <li>AWS::ElasticLoadBalancingV2::LoadBalancer</li>
  <li>AWS::ElasticLoadBalancingV2::Listener</li>
  <li>AWS::ElasticLoadBalancingV2::ListenerRule</li>
  <li>AWS::ElasticLoadBalancingV2::TargetGroup</li>
  <li>AWS::AutoScaling::ScalingPolicy</li>
  <li>AWS::CloudWatch::Alarm</li>
</ul>
