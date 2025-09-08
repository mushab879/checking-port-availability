Step 1: Python Script

target = "127.0.0.1"

ports = [21, 22, 25, 80, 443]

print(f"Scanning {target}...")

for port in ports:
    s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
    s.settimeout(1)  # 1-second timeout
    result = s.connect_ex((target, port))
    if result == 0:
        print(f"Port {port} is OPEN")
    else:
        print(f"Port {port} is CLOSED")
    s.close()

Step 2: Run the Script
python3 port_scanner.py

Step 3: Example Output

Scanning 127.0.0.1...
Port 21 is CLOSED
Port 22 is OPEN
Port 25 is CLOSED
Port 80 is OPEN
Port 443 is CLOSED
