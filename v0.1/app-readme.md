# Lightstep

### Description:

Lightstep satellites are used to report telemetry data to and store that data for recall from the SaaS application Lightstep manages.  
 
## Configuration:

In order to configure the satellite appropriately, please consult https://docs.lightstep.com/docs/satellite-configuration-parameters.  If you have questions, or need some human help, please contact support@lightstep.com.

## Usage
* This will run a Lightstep satellite within Rancher.  The satellite will be listening for data on 8182 for unsecure HTTP traffic, or secure HTTP traffic that terminates it's secure status before it hits the satellite and on 8183 for secure HTTP traffic.  You should configure your tracers to write to this satellite service on either one of those ports.
