# Ticket 003 – Slow Computer Performance

## 1. Identify the Problem
User reported Windows workstation running slowly with multiple apps open.

## 2. Environment
- Windows 11 ARM (UTM on macOS)
- CPU: 8-core
- RAM: 16GB

## 3. Initial Observations
- High CPU and memory usage in Task Manager
- Multiple apps running simultaneously

## 4. Troubleshooting Steps Taken
- Opened Task Manager to identify resource-heavy processes
- Closed unnecessary applications
- Ended high-CPU background processes
- Disabled unnecessary startup apps

## 5. Resolution
System performance improved after removing unnecessary processes and optimizing startup applications.

## 6. Verification
- CPU and memory usage returned to normal
- User can open apps without lag

## 7. Root Cause
Too many apps running simultaneously and unnecessary startup processes consuming resources.

## 8. Prevention
- Educate user on closing unused apps
- Review startup applications periodically
- Monitor system performance regularly

## Screenshots
- Screenshot 1: High CPU/Memory usage
![High CPU/Memory usage](01-high-cpu-usage.png)
- Screenshot 2: Identified culprit process
- Screenshot 3: Optimized Task Manager
![Optimized Task Manager](03-optimized-task-manager.png)
- Screenshot 4: Normalized performance
![Normalized performace](04-normalized-performance.png)

