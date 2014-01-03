# Scope of hub

 - central entrypoint (database) for "tasks"
 - api for mutating tasks
 - hub for container provisioner's
 - decides which provisioner to give task to
 - has real time information on status of any given task
 - glues container provisioners to hub
 - database for all task requirements


# Public Task API

For now lets limit the scope of tasks to consumers who have the task id

GET /v1/task/:id/
RESPONSE
```
{
  id: '',
  status: '',
  links: {
    self: { href: '...' }
  },

  artifacts: {
    log: {
      status: 'complete',
      url: '...'
    },
  }
}
```
