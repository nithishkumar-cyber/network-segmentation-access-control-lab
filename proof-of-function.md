## Network Validation

### Ping & Connectivity Tests

- ❌ PC1 → PC2: Communication correctly restricted
- ✅ PC1 → PC3: Communication verified according to network policy
- ❌ PC2 → PC3: Communication correctly restricted


---

### Routing Tables

- Verified all static routes using `show ip route`
- Confirmed correct packet forwarding across segments

---

### Access Control Policies

- Verified ACL rules with `show access-lists`
- Hit counters confirmed that traffic was filtered according to design

---

### DHCP Validation

- PCs in dynamic subnets received IP addresses automatically
- Static IP assigned correctly for fixed host

---

### Summary

- Network policies enforced as intended
- Segmented communication verified between subnets
- Routing and DHCP configurations confirmed functional