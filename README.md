# System-Analysis-Learning-Notes
计算机软考系统分析师学习笔记


# 软连接步骤：
1. 管理员权限打开powershell
2. `Remove-Item .claude -Recurse -Force`
3. `New-Item -ItemType SymbolicLink -Path .claude -Target .agents`