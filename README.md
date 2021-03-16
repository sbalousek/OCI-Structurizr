# Structurizr Themes for Oracle Cloud Infrastructure (OCI)

Themes for adding OCI icons to [Structurizr](https://structurizr.com/) diagrams.  See the available
icon names at [this link](https://structurizr.com/help/theme?url=https://static.structurizr.com/themes/oracle-cloud-infrastructure-2020.04.30/theme.json).

## Example

```dsl
workspace "Example" {
    model "OCI" {
        User    = person         "OCI User"    "Uses Oracle Cloud Infrastructure"
        Compute = softwareSystem "OCI Compute" "Provides computational service (IaaS)" "Oracle Cloud Infrastructure - VM"
        User -> Compute "Uses"
    }
    views {
        systemlandscape "SystemLandscape" {
            include *
            autoLayout
        }
        themes "https://raw.githubusercontent.com/sbalousek/OCI-Structurizr/master/light.json"
    }
}
```
