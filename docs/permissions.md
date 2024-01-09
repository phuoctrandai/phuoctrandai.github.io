---
layout: page
permalink: /permissions
---

# Envault Permission System
Permissions in Envault are based on [Access Control Lists (ACL's)](https://en.wikipedia.org/wiki/Access-control_list) and use [Create, Read, Update, Delete (CRUD)](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete) policies to provide access to the node tree. \
ACL's are inherited from the parent node unless explicitly defined on the node through the Role definition. This allows for granular access to resources within the node tree. 

Envault has three classes of users:

## Hub User
- Role based access
- Can modify own account details
- Can create, read, update, and delete API keys for user assigned roles
- Can create, read, update, and delete nodes within the roles boundaries

## Hub Admin
- Update Hub details and configuration
- Invite and remove Users
- Create and assign Roles to Users and API keys
- Can self assign Roles, role policy will apply where denials exist
- All features of Hub User

## App Admin
- Create New Hubs
- Must be part a Hub member to create nodes with ownership requirements:
  - Chart
  - Dashboard
  - Timelapse
- All features of Hub Admin
