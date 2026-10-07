# Zupra ERP v16
Frappe v16 + ERPNext v16 (full source).
Requires: Python 3.14, Node 24, MariaDB 11.8+, Redis.

## Restore on a new machine
git clone https://github.com/zupratechllp-hub/Zupra_ERP_v16.git
cd Zupra_ERP_v16
bench setup env --python python3.14
bench setup requirements
bench setup redis
bench setup procfile
bench build
bench new-site SITE_NAME --install-app erpnext
bench use SITE_NAME
bench start
