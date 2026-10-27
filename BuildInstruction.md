# 1C External Processor (.epf) Build Guide (1-Minute Setup)

This guide walks you through building the `СжатиеКартинокНоменклатуры.epf` external data processor in 1C:Enterprise Configurator in just **1 to 2 minutes**.

The managed form is equipped with a **self-generating UI engine**: you do **not** need to manually add attributes, table columns, groups, or commands!

---

## ⚡ Fast Assembly in 1C Configurator

### Step 1. Create a New External Processor
1. Launch **1C:Enterprise Configurator** (with any infobase).
2. From the main menu, select: **File → New...**
3. Select **External Data Processor** (Внешняя обработка) and click **OK**.
4. In the properties window, fill in:
   - **Name**: `СжатиеКартинокНоменклатуры`
   - **Synonym**: `Image Compression for Nomenclature (UT 11 / ERP)`

---

### Step 2. Paste the Object Module
1. In the data processor window, click **Actions → Open Object Module** (or right-click root → *Object Module*).
2. Copy the entire code from [**`МодульОбъекта.bsl`**](./МодульОбъекта.bsl) (`Ctrl + A` → `Ctrl + C`).
3. Paste it into the editor (`Ctrl + A` → `Ctrl + V`).
4. Close the object module editor.

---

### Step 3. Create the Managed Form (Self-Generating)
1. In the data processor window under **Forms** (Формы), click the **Add** button (`+`).
2. In the form creation wizard:
   - Form Type: **Main Data Processor Form** (selected by default).
   - Click **Finish** (Готово) directly without altering attributes.
3. In the form designer, switch to the **Module** tab at the bottom.
4. Copy the entire code from [**`МодульФормы.bsl`**](./МодульФормы.bsl) (`Ctrl + A` → `Ctrl + C`).
5. Paste it into the form module editor (`Ctrl + A` → `Ctrl + V`).
6. Press **`Ctrl + F7`** to run a syntax check (0 errors).

---

### Step 4. Save as .epf
1. Select **File → Save As...** (`Ctrl + S`).
2. Save as: **`СжатиеКартинокНоменклатуры.epf`**.

The external processor is fully built and ready for production use.
