---
description: 0Resmon RC Car Installation Document and Basic Concepts
---

# Installation

This installation guide covers both <mark style="color:red;">ESX</mark>, <mark style="color:blue;">QBCore</mark> and <mark style="color:yellow;">QBOX</mark> frameworks.

<table>
    <thead>
        <tr>
            <th width="202">Resource</th>
            <th>Source</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>ox_lib</td>
            <td><a href="https://github.com/overextended/ox_lib/releases/download/v3.27.0/ox_lib.zip">Download</a></td>
        </tr>
    </tbody>
</table>

### Target System

The system can work with <mark style="color:blue;">**ox\_target**</mark> and <mark style="color:red;">**qb-target**</mark> plugins. Or you can use it with drawtext

### Supported Inventories

* qb-inventory
* ox\_inventory
* ps-inventory
* lj-inventory
* tgiann-inventory
* codem-inventory

# Insert The SQL

Insert the file called `insert-me.sql` that comes inside the script file

## Setup For Inventories

{% tabs %}
    {% tab title="ox_inventory" %}
        Open the <mark style="color:blue;">**ox\_inventory/data/items.lua**</mark> file. And place the following code.

        <pre class="language-lua">
            <code class="lang-lua">
                ['rc_monster'] = {
                    label = "RC Monster",
                    weight = 1500,
                    stack = false,
                    close = true,
                    description = "RC car in 4x4 type",
                    client = {
                        image = "rc_monster.png",
                    }
                },

                ['rc_ruiner'] = {
                    label = "RC Ruiner",
                    weight = 1500,
                    stack = false,
                    close = true,
                    description = "RC car in 4x4 type",
                    client = {
                        image = "rc_ruiner.png",
                    }
                },

                ['rc_sultanrs'] = {
                    label = "RC Sultan RS",
                    weight = 1500,
                    stack = false,
                    close = true,
                    description = "RC car in 4x4 type",
                    client = {
                        image = "rc_sultanrs.png",
                    }
                },

                ['rc_bandito'] = {
                    label = "RC Bandito",
                    weight = 1500,
                    stack = false,
                    close = true,
                    description = "RC car in 4x4 type",
                    client = {
                        image = "rc_bandito.png",
                    }
                },

                ['rc_bandito_offroad'] = {
                    label = "RC Bandito Offroad",
                    weight = 1500,
                    stack = false,
                    close = true,
                    description = "RC car in 4x4 type",
                    client = {
                        image = "rc_bandito_offroad.png",
                    }
                },

                ['rc_bandito_trophy'] = {
                    label = "RC Bandito Trophy",
                    weight = 1500,
                    stack = false,
                    close = true,
                    description = "RC car in 4x4 type",
                    client = {
                        image = "rc_bandito_trophy.png",
                    }
                },

                ['rc_bandito_gang'] = {
                    label = "RC Bandito Gang",
                    weight = 1500,
                    stack = false,
                    close = true,
                    description = "RC car in 4x4 type",
                    client = {
                        image = "rc_bandito_gang.png",
                    }
                },

                ['rc_bandito_big'] = {
                    label = "RC Bandito Big",
                    weight = 1500,
                    stack = false,
                    close = true,
                    description = "RC car in 4x4 type",
                    client = {
                        image = "rc_bandito_big.png",
                    }
                },

                ['rc_bandito_midnight'] = {
                    label = "RC Bandito Midnight",
                    weight = 1500,
                    stack = false,
                    close = true,
                    description = "RC car in 4x4 type",
                    client = {
                        image = "rc_bandito_midnight.png",
                    }
                },

                ['rc_advancedcamera'] = {
                    label = "Advanced Camera Extension",
                    weight = 500,
                    stack = false,
                    close = false,
                    description = "Night vision plugin for RC car",
                    client = {
                        image = "thermalscope_attachment.png",
                    }
                },

                ['rc_nitrous'] = {
                    label = "Nitrous Extension",
                    weight = 500,
                    stack = false,
                    close = false,
                    description = "Nitrous plugin for RC car",
                    client = {
                        image = "thermalscope_attachment.png",
                    }
                },

                ['rc_battery'] = {
                    label = "Battery Extension",
                    weight = 500,
                    stack = false,
                    close = false,
                    description = "Battery plugin for RC car",
                    client = {
                        image = "thermalscope_attachment.png",
                    }
                },

                ['rc_bomb'] = {
                    label = "Bomb Extension",
                    weight = 500,
                    stack = false,
                    close = false,
                    description = "Bomb plugin for RC car",
                    client = {
                        image = "thermalscope_attachment.png",
                    }
                },

                ['rc_jump'] = {
                    label = "Jump Extension",
                    weight = 500,
                    stack = false,
                    close = false,
                    description = "Jump plugin for RC car",
                    client = {
                        image = "thermalscope_attachment.png",
                    }
                },

                ['rc_identifier'] = {
                    label = "Scan Identifier Extension",
                    weight = 500,
                    stack = false,
                    close = false,
                    description = "Scan identifier plugin for RC car",
                    client = {
                        image = "thermalscope_attachment.png",
                    }
                },

                ['rc_teaser'] = {
                    label = "Teaser Extension",
                    weight = 500,
                    stack = false,
                    close = false,
                    description = "Teaser plugin for RC car",
                    client = {
                        image = "thermalscope_attachment.png",
                    }
                },

                ['copper'] = {
                    label = "Copper",
                    weight = 100,
                    stack = false,
                    close = false,
                    description = "Nice piece of metal that you can probably use for something",
                    client = {
                        image = "copper.png",
                    }
                },

                ['iron'] = {
                    label = "Iron",
                    weight = 100,
                    stack = false,
                    close = false,
                    description = "Handy piece of metal that you can probably use for something",
                    client = {
                        image = "iron.png",
                    }
                },

                ['silver'] = {
                    label = "Silver",
                    weight = 100,
                    stack = false,
                    close = false,
                    description = "Handy piece of metal that you can probably use for something",
                    client = {
                        image = "silver.png",
                    }
                },

                ['emerald'] = {
                    label = "Emerald",
                    weight = 100,
                    stack = false,
                    close = false,
                    description = "Handy piece of metal that you can probably use for something",
                    client = {
                        image = "emerald.png",
                    }
                },

                ['screw'] = {
                    label = "Screw",
                    weight = 100,
                    stack = false,
                    close = false,
                    description = "Handy piece of metal that you can probably use for something",
                    client = {
                        image = "screw.png",
                    }
                }
            </code>
        </pre>
    {% endtab %}

    {% tab title="qb-inventory, lj-inventory, ps-inventory" %}
        The best thing about these inventories is that their infrastructure is qb-inventory. That's why the installations are the same.

        Place these items in items.lua in your inventories. (qb-inventory to qb-core/shared/items.lua)

        <pre class="language-lua">
            <code class="lang-lua">
                rc_monster                   = { name = 'rc_monster', label = 'RC Monster', weight = 1500, type = 'item', image = 'rc_monster.png', unique = true, useable = true, shouldClose = true, description = 'A RC Car' },
                rc_ruiner                    = { name = 'rc_ruiner', label = 'RC Ruiner', weight = 1500, type = 'item', image = 'rc_ruiner.png', unique = true, useable = true, shouldClose = true, description = 'A RC Car' },
                rc_sultanrs                  = { name = 'rc_sultanrs', label = 'RC Sultan RS', weight = 1500, type = 'item', image = 'rc_sultanrs.png', unique = true, useable = true, shouldClose = true, description = 'A RC Car' },
                rc_bandito                   = { name = 'rc_bandito', label = 'RC Bandito', weight = 1500, type = 'item', image = 'rc_bandito.png', unique = true, useable = true, shouldClose = true, description = 'A RC Car' },
                rc_bandito_offroad           = { name = 'rc_bandito_offroad', label = 'RC Bandito Offroad', weight = 1500, type = 'item', image = 'rc_banrc_bandito_offroaddito.png', unique = true, useable = true, shouldClose = true, description = 'A RC Car' },
                rc_bandito_trophy            = { name = 'rc_bandito_trophy', label = 'RC Bandito Trophy', weight = 1500, type = 'item', image = 'rc_bandito_trophy.png', unique = true, useable = true, shouldClose = true, description = 'A RC Car' },
                rc_bandito_gang              = { name = 'rc_bandito_gang', label = 'RC Bandito Gang', weight = 1500, type = 'item', image = 'rc_bandito_gang.png', unique = true, useable = true, shouldClose = true, description = 'A RC Car' },
                rc_bandito_big               = { name = 'rc_bandito_big', label = 'RC Bandito Big', weight = 1500, type = 'item', image = 'rc_bandito_big.png', unique = true, useable = true, shouldClose = true, description = 'A RC Car' },
                rc_bandito_midnight          = { name = 'rc_bandito_midnight', label = 'RC Bandito Midnight', weight = 1500, type = 'item', image = 'rc_bandito_midnight.png', unique = true, useable = true, shouldClose = true, description = 'A RC Car' },
                
                rc_advancedcamera            = { name = 'rc_advancedcamera', label = 'Advanced Camera Extentation', weight = 500, type = 'item', image = 'rc_advancedcamera.png', unique = false, useable = false, shouldClose = false, description = 'Night vision plugin for RC car' },
                rc_nitrous                   = { name = 'rc_nitrous', label = 'Nitrous Extentation', weight = 500, type = 'item', image = 'rc_nitrous.png', unique = false, useable = false, shouldClose = false, description = 'Nitrous plugin for RC car' },
                rc_battery                   = { name = 'rc_battery', label = 'Battery Extentation', weight = 500, type = 'item', image = 'rc_battery.png', unique = false, useable = false, shouldClose = false, description = 'Battery plugin for RC car' },
                rc_bomb                      = { name = 'rc_bomb', label = 'Bomb Extentation', weight = 500, type = 'item', image = 'rc_bomb.png', unique = false, useable = false, shouldClose = false, description = 'Bomb plugin for RC car' },
                rc_jump                      = { name = 'rc_jump', label = 'Jump Extentation', weight = 500, type = 'item', image = 'rc_jump.png', unique = false, useable = false, shouldClose = false, description = 'Jump plugin for RC car' },
                rc_identifier                = { name = 'rc_identifier', label = 'Scan Identifier Extentation', weight = 500, type = 'item', image = 'rc_identifier.png', unique = false, useable = false, shouldClose = false, description = 'Scan identifier plugin for RC car' },
                rc_teaser                    = { name = 'rc_teaser', label = 'Teaser Extentation', weight = 500, type = 'item', image = 'rc_teaser.png', unique = false, useable = false, shouldClose = false, description = 'Teaser plugin for RC car' },
                copper                       = { name = 'copper', label = 'Copper', weight = 100, type = 'item', image = 'copper.png', unique = false, useable = false, shouldClose = false, description = 'Nice piece of metal that you can probably use for something' },
                iron                         = { name = 'iron', label = 'Iron', weight = 100, type = 'item', image = 'iron.png', unique = false, useable = false, shouldClose = false, description = 'Handy piece of metal that you can probably use for something' },
                silver                       = { name = 'silver', label = 'Silver', weight = 100, type = 'item', image = 'silver.png', unique = false, useable = false, shouldClose = false, description = 'Handy piece of metal that you can probably use for something' },
                emerald                      = { name = 'emerald', label = 'Emeral', weight = 100, type = 'item', image = 'emerald.png', unique = false, useable = false, shouldClose = false, description = 'Handy piece of metal that you can probably use for something' },
                screw                        = { name = 'screw', label = 'Screw', weight = 100, type = 'item', image = 'screw.png', unique = false, useable = false, shouldClose = false, description = 'Handy piece of metal that you can probably use for something' },
            </code>
        </pre>

        Open your inventory javascript file. And search for the <mark style="color:blue;">**FormatItemInfo**</mark> function and place this code in the if loop within that function. There should be a <mark style="color:blue;">**metadata.js**</mark> file in <mark style="color:blue;">**qs-inventory**</mark>, do the same process there.

        ```javascript
            } else if (itemData.name == 'rc_monster' || itemData.name == 'rc_ruiner' || itemData.name == 'rc_sultanrs' || itemData.name == 'rc_bandito' || itemData.name == 'rc_bandito_offroad' || itemData.name == 'rc_bandito_trophy' || itemData.name == 'rc_bandito_gang' || itemData.name == 'rc_bandito_big' || itemData.name == 'rc_bandito_midnight') {
                $(".item-info-title").html("<p>" + itemData.label + "</p>");
                $(".item-info-description").html(
                    "<p><strong>Serie Number: </strong><span>" +
                    itemData.info.serie
            );
        ```

        **For New qb-inventory**

        ```javascript
        case "rc_monster":
            return `<p><strong>Serie Number: </strong><span>${itemData.info.serie}</span></p>`;
        case "rc_ruiner":
            return `<p><strong>Serie Number: </strong><span>${itemData.info.serie}</span></p>`;
        case "rc_sultanrs":
            return `<p><strong>Serie Number: </strong><span>${itemData.info.serie}</span></p>`;
        case "rc_bandito":
            return `<p><strong>Serie Number: </strong><span>${itemData.info.serie}</span></p>`;
        case "rc_bandito_offroad":
            return `<p><strong>Serie Number: </strong><span>${itemData.info.serie}</span></p>`;
        case "rc_bandito_trophy":
            return `<p><strong>Serie Number: </strong><span>${itemData.info.serie}</span></p>`;
        case "rc_bandito_gang":
            return `<p><strong>Serie Number: </strong><span>${itemData.info.serie}</span></p>`;
        case "rc_bandito_big":
            return `<p><strong>Serie Number: </strong><span>${itemData.info.serie}</span></p>`;
        case "rc_bandito_midnight":
            return `<p><strong>Serie Number: </strong><span>${itemData.info.serie}</span></p>`;
        ```
    {% endtab %}

    {% tab title="codem-inventory" %}
        Add this code to the if condition in the codem-inventory/config/metadata.js file located in the inventory.

        ```javascript
        } else if (item.name.match("rc_monster") || item.name.match("rc_ruiner") || item.name.match("rc_sultanrs") || item.name.match("rc_bandito") || item.name.match("rc_bandito_offroad") || item.name.match("rc_bandito_trophy") || item.name.match("rc_bandito_gang") || item.name.match("rc_bandito_big") || item.name.match("rc_bandito_midnight")) {
            let infoData = [
                { label: "Serie Number: ", value: iteminfo.serie },
            ]
            returnString = infoData;
        ```
    {% endtab %}

    {% tab title="tgiann-inventory" %}
        Find the metadata.js file and add this code to the item list in the qbItemInfo function.

        ```javascript
        } else if (itemData.name == 'rc_monster' || itemData.name == 'rc_ruiner' || itemData.name == 'rc_sultanrs' || itemData.name == 'rc_bandito' || itemData.name == 'rc_bandito_offroad' || itemData.name == 'rc_bandito_trophy' || itemData.name == 'rc_bandito_gang' || itemData.name == 'rc_bandito_big' || itemData.name == 'rc_bandito_midnight') {
            html = `
            <div class="item_info_container">
                <div class="item_info_row">
                    <div class="item_info_row_left">Serie Number: </div>
                    <div class="item_info_row_right">${itemData.info.serie}</div>
                </div>
            </div>`;
        ```
    {% endtab %}
{% endtabs %}

### Give Item Commands

Add this in the `giveitem` command in the inventory you are using

```lua
elseif itemData['name'] == 'rc_monster' or itemData['name'] == 'rc_ruiner' or itemData['name'] == 'rc_sultanrs' or itemData['name'] == 'rc_bandito' or itemData['name'] == 'rc_bandito_offroad' or itemData['name'] == 'rc_bandito_trophy' or itemData['name'] == 'rc_bandito_gang' or itemData['name'] == 'rc_bandito_big' or itemData['name'] == 'rc_bandito_midnight' then
    exports['0r-rccar']:CreateNewVehicle(id, itemData['name'], 1, false, nil, true)
    return
```
