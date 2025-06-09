# canmatrix_webapp

A Streamlit webapp for the [canmatrix](https://github.com/ebroecker/canmatrix) Python package.

## Environment Setup

* Run `scripts/venv_setup.bat` to create and activate a virtual environment with all dependencies.

## Installation

1. Clone this repository.
2. Set up the environment as above.
3. (Optional) Build the wheel:
   `scripts/build_wheel_package.bat`

## Usage

### Launch the Web Application

You can start the web application using the provided launcher:

```sh
python -m canmatrix_webapp.run_web_app
```

#### Optional Arguments

- `--server-address ADDRESS`
  Address to bind the Streamlit server (default: system FQDN)
- `--server-port PORT`
  Port to run the Streamlit server on (default: 8502)

Example:

```sh
python -m canmatrix_webapp.run_web_app --server-address 127.0.0.1 --server-port 8502
```

### Features

- Upload CAN matrix files in various formats (DBC, ARXML, KCD, FIBEX, XLS, XLSX, XML)
- Explore loaded matrices, view ECUs, frames, and signals
- Export matrices to supported formats

## Documentation

- Build docs locally:
  `scripts/local_mkdoc_build.bat`

---
