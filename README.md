# sat-capsule-helper
Project to help on Satellite setup to connect with a Capsule

#Rationale
To connect to a capsule a lot of work is needed on Satellite to create some 
entities. The purpose of this project is to help on this.
The info is based on this [gist](https://gist.github
.com/omaciel/eecee74971e6f1e948a6), but for the use case of installing 
capsule on other machine instead of on the same one as main Satellite.

# What it will do

1. Create **DEV** lifecycle-environment for for **Default Organization** with 
**Library as prior environment**;
2. Import RH Manifest;
3. Enable **Red Hat Enterprise Linux 7 Server RPMs x86_64 7.3**;
4. Enable **Red Hat Satellite Tools 6.2 for RHEL 7 Server RPMs x86_64**;
5. Enable **Red Hat Satellite Capsule 6.2 for RHEL 7 Server RPMs x86_64**;
6. Synchonize repos;
7. Create Content View **RHEL 7 CAPSULE CV**;
8. Add 3 previous repo to **RHEL 7 CAPSULE CV**;
9. Publish **RHEL 7 CAPSULE CV**;
10. Promote **RHEL 7 CAPSULE CV** to **DEV**;
11. Create Host Collection **Capsule HC**;
12. Create Activation Key **ak-capsule-7**;
13. Add Subscriptions **Red Hat Employee Subscription** and **Red Hat 
Satellite Employee Subscription** to **ak-capsule-7**;
14. Add **Capsule HC** to **ak-capsule-7**;

