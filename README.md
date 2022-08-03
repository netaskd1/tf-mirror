# tf-mirror-proto

```terraform
terraform {
  required_providers {
    azurerm = {
      source  = "terraform-registry.company.com/hashicorp/azurerm"
      version = "=2.97.0"
    }
    
  }
}

# Configure the Microsoft Azure Provider
provider "azurerm" {
  features {}
}
```


# tf-mirror

```terraform
MIRROR="https://terraform-mirror.yandexcloud.net/"

cat << EOF >| ~/.terraformrc
provider_installation {
  network_mirror {
    url = "${MIRROR}"
    include = ["registry.terraform.io/*/*"]
  }
  direct {
    exclude = ["registry.terraform.io/*/*"]
  }
}
EOF
```

```terraform
terraform {
  required_providers {
    aws = {
      source  = "hashicorp/aws"
      version = "~> 4.16.0"
    }
    azurerm = {
      source  = "hashicorp/azurerm"
      version = "~> 2.97.0"
    }
  }
}
provider "ad" {}
provider "archive" {}
provider "aws" {}
provider "awscc" {}
provider "azuread" {}
provider "azurerm" {}
provider "azurestack" {}
provider "boundary" {}
provider "cloudinit" {}
provider "consul" {}
provider "dns" {}
provider "external" {}
provider "google" {}
provider "google-beta" {}
provider "googleworkspace" {}
provider "hcp" {}
provider "hcs" {}
provider "helm" {}
provider "http" {}
provider "kubernetes" {}
provider "kubernetes-alpha" {}
provider "local" {}
provider "nomad" {}
provider "null" {}
provider "oci" {}
provider "opc" {}
provider "oraclepaas" {}
provider "random" {}
provider "salesforce" {}
provider "template" {}
provider "terraform" {}
provider "tfe" {}
provider "time" {}
provider "tls" {}
provider "vault" {}
provider "vsphere" {}
provider "hashicups" {}
```

All providers

```terraform
terraform {
  required_providers {
    aws = {
      source  = "hashicorp/aws"
      version = "~> 4.16.0"
    }
    azurerm = {
      source  = "hashicorp/azurerm"
      version = "~> 2.97.0"
    }
    alicloud = {
      source = "aliyun/alicloud"
    }
    yandex = {
      source = "yandex-cloud/yandex"
    }
  }
}
provider "aci" {}
provider "acme" {}
provider "ad" {}
provider "akamai" {}
provider "alicloud" {}
provider "archive" {}
provider "arukas" {}
provider "atlas" {}
provider "auth0" {}
provider "avi" {}
provider "aviatrix" {}
provider "aws" {}
provider "awscc" {}
provider "azure" {}
provider "azuread" {}
provider "azuredevops" {}
provider "azurerm" {}
provider "azurestack" {}
provider "baiducloud" {}
provider "bigip" {}
provider "bitbucket" {}
provider "boundary" {}
provider "brightbox" {}
provider "checkpoint" {}
provider "chef" {}
provider "cherryservers" {}
provider "circonus" {}
provider "ciscoasa" {}
provider "clc" {}
provider "cloudamqp" {}
provider "cloudflare" {}
provider "cloudinit" {}
provider "cloudscale" {}
provider "cloudstack" {}
provider "cobbler" {}
provider "cohesity" {}
provider "constellix" {}
provider "consul" {}
provider "datadog" {}
provider "digitalocean" {}
provider "dme" {}
provider "dns" {}
provider "dnsimple" {}
provider "docker" {}
provider "dome9" {}
provider "dyn" {}
provider "ecl" {}
provider "equinix" {}
provider "exoscale" {}
provider "external" {}
provider "fakewebservices" {}
provider "fastly" {}
provider "flexibleengine" {}
provider "fortios" {}
provider "genymotion" {}
provider "github" {}
provider "gitlab" {}
provider "google" {}
provider "googleworkspace" {}
provider "grafana" {}
provider "gridscale" {}
provider "hcloud" {}
provider "hcp" {}
provider "hcs" {}
provider "hedvig" {}
provider "helm" {}
provider "heroku" {}
provider "http" {}
provider "huaweicloud" {}
provider "huaweicloudstack" {}
provider "icinga2" {}
provider "ignition" {}
provider "incapsula" {}
provider "influxdb" {}
provider "infoblox" {}
provider "jdcloud" {}
provider "ksyun" {}
provider "kubernetes" {}
provider "lacework" {}
provider "launchdarkly" {}
provider "librato" {}
provider "linode" {}
provider "local" {}
provider "logentries" {}
provider "logicmonitor" {}
provider "mailgun" {}
provider "metalcloud" {}
provider "mongodbatlas" {}
provider "mso" {}
provider "mysql" {}
provider "ncloud" {}
provider "netlify" {}
provider "newrelic" {}
provider "nomad" {}
provider "ns1" {}
provider "nsxt" {}
provider "null" {}
provider "nutanix" {}
provider "oci" {}
provider "okta" {}
provider "oktaasa" {}
provider "oneandone" {}
provider "onelogin" {}
provider "opc" {}
provider "opennebula" {}
provider "openstack" {}
provider "opentelekomcloud" {}
provider "opsgenie" {}
provider "oraclepaas" {}
provider "ovh" {}
provider "packet" {}
provider "pagerduty" {}
provider "panos" {}
provider "postgresql" {}
provider "powerdns" {}
provider "prismacloud" {}
provider "profitbricks" {}
provider "pureport" {}
provider "rabbitmq" {}
provider "rancher" {}
provider "rancher2" {}
provider "random" {}
provider "rightscale" {}
provider "rubrik" {}
provider "rundeck" {}
provider "runscope" {}
provider "salesforce" {}
provider "scaleway" {}
provider "sdm" {}
provider "selectel" {}
provider "selvpc" {}
provider "signalfx" {}
provider "skytap" {}
provider "softlayer" {}
provider "spotinst" {}
provider "stackpath" {}
provider "statuscake" {}
provider "sumologic" {}
provider "telefonicaopencloud" {}
provider "template" {}
provider "tencentcloud" {}
provider "terraform" {}
provider "tfe" {}
provider "thunder" {}
provider "time" {}
provider "tls" {}
provider "triton" {}
provider "turbot" {}
provider "ucloud" {}
provider "ultradns" {}
provider "vault" {}
provider "vcd" {}
provider "venafi" {}
provider "vmc" {}
provider "vra" {}
provider "vra7" {}
provider "vsphere" {}
provider "vthunder" {}
provider "vultr" {}
provider "wavefront" {}
provider "yandex" {}
```
