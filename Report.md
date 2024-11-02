# DevOps Assignment: Debugging and Running a Dockerized Application

## App.py

### Issues and Fixes
- **Assumption**:
  - Using `socket.gethostname()` to capture the server’s hostname instead of relying on `request.headers.get()` for a client-provided username.
  - As the Flask application runs behind a reverse proxy (like Nginx), `request.remote_addr` may return the IP address of the proxy server instead of the actual client.
- **MAC Address Retrieval**:
  - Filter interfaces to avoid loopback (`lo`).
  - Check for valid MAC addresses.

---

## Python App Dockerfile

### Issues and Fixes
- **Corrections**:
  - `"eight thousand"` should be `8000`.
  - `"pythn"` should be `"python"`.
  - File paths are inconsistent: `appp` vs `/app`.
  - Wrong filename: `appy.py` should be `app.py`.
  - The correct library is `netifaces` (not `netiface`).
- **Improvement**:
  - Use `python:3.9-slim` for a smaller image size as per requirement.

---

## Nginx Config File

### Issues and Fixes
- **Corrections**:
  - The correct directive is `worker_processes` (with an "es").
  - There is a typo in `mime.typess`; it should be `mime.types`.
  - There is a typo in `default_typ`; it should be `default_type`.

---

## Nginx Dockerfile

### Issues and Fixes
- **Corrections**:
  - The correct tag is `nginx:latest` (remove the extra 's').
  - `nginix.conf` should be `nginx.conf`.
  - `/usr/share/nginx/htmll` should be `/usr/share/nginx/html`. (Can remove this line if wanting to serve the default HTML page).
  - Use the numeric `EXPOSE 80`, not a string.
  - `"daemon of;"` should be `daemon off;`.

---

## Docker Compose File

### Issues and Fixes
- **Corrections**:
  - Port numbers should be in numeric form.
  - The file path `nginx.confi` was incorrect; it should be `nginx.conf`.
  - The correct network driver is `bridge`.
  - `compelex_option` appears to be a typo.


## Bonus Points: Cloud Deployment

- The application has been successfully deployed on **AWS** with the following public IP address:
  - **[13.235.83.44](https://13.235.83.44)**
- The deployment includes:
  - A **self-signed SSL certificate** to secure the Flask application.
  - The Nginx reverse proxy configured to forward requests to the Flask app running on port 8000.
- To access the application:
  - Use the following URL: [https://13.235.83.44](https://13.235.83.44)
  - You may need to bypass a browser security warning due to the **self-signed certificate**.

