## Exercise 3: Creating a device group

Duration: 10 minutes

Device groups allow you to create logical groupings of IoT Devices in the field by the properties that defined them. In this case, we will want to create a device set that contains only the rod pumps located in the state of Texas.

### Task 1: Create a device group using a filter

1. In the left-hand menu, select the _Device groups_ menu item. You will see a single default device group in the list (_Rod Pump - All devices_). Select the _+ New_ button in toolbar.

![alt text](https://raw.githubusercontent.com/CloudLabs-MCW/MCW-Predictive-Maintenance-for-remote-field-devices/stage/Hands-on%20lab/media/device-set-list.png)

2. In the field, all Texas pumps are located in the *192.168.1.* subnet, so we will create a filter to include only those pumps in this device group. Create the Device group with the filter as described in the following table. Feel free to _Run query_ to see the devices included, then select _Save_ from the toolbar:

![alt text](https://raw.githubusercontent.com/CloudLabs-MCW/MCW-Predictive-Maintenance-for-remote-field-devices/stage/Hands-on%20lab/media/new-device-set.png)

    | Field               | Value                      |
    | ------------------- | -------------------------- |
    | Device Group Name (in header) | Texas Rod Pumps            |
    | Description (in header)       | Rod pumps located in Texas |
    | Scope Device Template     | Rod Pump           |
    | Filter: Property | IP Address                 |
    | Filter: Operator | contains                   |
    | Filter: Value    | 192.168.1.                 |

3. Once the Device group is saved, you are able to act upon this group of devices as a single unit within IoT Central.