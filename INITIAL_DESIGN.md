# Scope of hub

 - central entrypoint (database) for "tasks"
 - api for mutating tasks
 - hub for container provisioner's
 - decides which provisioner to give task to
 - has real time information on status of any given task
 - glues container provisioners to hub
 - database for all task requirements


# Public Task Mutation API
  
  - POST /v1/task { ... }

# Private Container API

  - 
