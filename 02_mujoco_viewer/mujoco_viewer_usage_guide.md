# How to Open and View XML Files in MuJoCo Viewer

Here are 3 simple methods to launch and view your XML files in the MuJoCo viewer.

---

### Method 1: Interactive Drag and Drop

1. Open your terminal and run:
   ```bash
   python3 -m mujoco.viewer
   ```
2. A blank MuJoCo viewer window will open.
3. Drag and drop your `.xml` file directly into the viewer window.

> **Note:** Depending on your setup, you might need to use `python` instead of `python3`.

---

### Method 2: Command Line Argument

You can directly load a file by passing its complete path using the `--mjcf` flag.

**Syntax:**
```bash
python3 -m mujoco.viewer --mjcf=(complete_path_to_xml)
```

**Example:**
```bash
python3 -m mujoco.viewer --mjcf=/Users/mubashir/Desktop/hello.xml
```

> **Note:** Make sure to include two hyphens (`--`) before `mjcf`.

---

### Method 3: Python Script Execution

You can run a script from inside your project folder where your XML file and Python script reside together.

1. Navigate to your project folder:
   ```bash
   cd 02_mujoco_viewer
   ```

2. Make sure both `hello.xml` and `template_mujoco_viewer.py` are in this folder.

3. Run the script:
   ```bash
   python3 template_mujoco_viewer.py
   ```