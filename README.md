# 🧰 qb-inventory (Modified Version)

This is a customized version of `qb-inventory` for the QBCore framework. It introduces major improvements:

- 💸 **Cash as an inventory item**  
- 🎒 **Back item props for immersive carrying visuals**  
- 🖥️ **A redesigned, modern UI**

---

## 🚀 Features

- ✅ Cash is now a physical item (`cash`) that can be dropped, traded, or stored in inventory.
- ✅ Items like bags, large tools, and certain weapons show props on the player's back when carried.
- ✅ Fully redesigned and responsive inventory UI.

---

## 📦 Installation

1. Replace your existing `qb-inventory` with this modified version.
2. **Add the `cash` item** to your shared items in `qb-core/shared/items.lua`.

---

## 🔧 Add `cash` Item

In your `qb-core/shared/items.lua`, insert the following:

```lua
['cash'] = {
    name = 'cash',
    label = 'Cash',
    weight = 0,
    type = 'item',
    image = 'cash.png',
    unique = false,
    useable = false,
    shouldClose = true,
    combinable = nil,
    description = 'Some loose cash you can carry or trade.',
    stack = true,
    close = true,
    server = false
},
