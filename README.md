# Resource Optimization Telemetry Agent

The agent collects local CPU, memory, disk, network, battery, and process metrics and sends them to the Flask backend after the user signs in.

## Configuration

The agent asks for the backend URL on the login screen. Use:

- Local backend: `http://127.0.0.1:5001`
- Deployed backend: your HTTPS API URL, for example `https://api.example.com`

The agent stores only the email and backend URL in the user's home directory. It does not save the password.

## Run from source

```powershell
python -m pip install -r requirement.txt
python agent.py
```

The downloadable Windows and Linux artifacts are served by the backend from its `downloads` directory.
