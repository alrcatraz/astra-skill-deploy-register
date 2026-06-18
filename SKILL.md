---
name: deploy-register
description: "Mandatory registration checklist after deploying a new service or facility: register in service inventory, attach health checks, clean up residuals."
category: devops
version: 1.0.0
---

# deploy-register

## Trigger Conditions

This skill is automatically loaded when the task involves:
- Deploying, installing a service, starting a service, registering a service
- Configuring a service, exposing a port, going live, publishing
- Any new service, MCP server, CLI tool, or other facility deployed for the agent

## Checklist

- [ ] **Has the service been registered in the service inventory?**
  - Name, deployment location, port, purpose, health check method
- [ ] **Has it been wired into automated health checks?**
  - Yes → write or update the check script
  - No → file a to-do item
- [ ] **Are there old versions, old processes, or old configurations to clean up?**
- [ ] **Were temporary files created during deployment?** Have they been cleaned up?
- [ ] **If this service is removed in the future, what needs to be cleaned?** Database records, check scripts, reference documentation.

## Pitfalls

1. **Deploy and walk away = management black hole.** When an unregistered service fails, you won't even know it exists.
2. **The service inventory is not a one-time thing.** When removing a service, it must be de-registered and all references thoroughly cleaned.
