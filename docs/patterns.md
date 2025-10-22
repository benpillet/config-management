reproducibility vs adhoc/manual changes
workflow: get it working by hand, automate it
over reaching change usually doesn't work
pull a change in from a single host then refactoring
UI for authentication/job lifecycle tracking/sharing; rundeck/jenkins
immutable infrastructure != no config management
challenges of running branches of automation on systems to see if they're valid. inevitably there will be out-of-sync resources, but "finishing" is is success
orchestration vs choreography -- centralized management/proscriptive -- individual participlation by a node
making dashboards to view entropy as technical debt
cluster/inventory centric with playbooks vs host/node centric models
package -> files -> services
db schema/users -> package -> files -> services -> monitoring
config files inside docker containers instead of in central ansible repo
templating languages: jinja sucks; erb is passable;
declarative languages vs imperative
Greenspun's 10th law in relation to config files; it starts off with 'include'
secrets management
no deeply nested hiera files
automatic tags and filtering target tasks and nodes
config in a db vs files
showing file diffs
golden image anti pattern
managing state files
Idempotency
a clean dry run is necessary but not sufficient
resource/provider split
file concat; challenges of having different file parts in different modules
dev laptop/workstation config management
control tower
facter ohai
delete unmanaged files in a directory or unmanaged users
manage single lines in files or whole files; lens
role/ profile; wrapper recipe
single instance on a server versus multiple instances on the server for things like Ssh
translate to eat each option for a service in to the configuration management language or manage course concepts like config files; augeas as intermediate
command line parameters for awscli are really concepts that should be abstracted; not just awscli but also Jenkins jobs
autosafe runs: pros/cons
do runs across a slice to reduce risk
managing artifacts: using a yum repo; managing a templates script inside cm
a instances are a projection of a cm
“target”, usually a node, but datadog-monitor #3 is a target too
difficulty managing api’s like databases
March Towards the horizon
speed The parade Attachment styles and Dev ops The trifecta for monitoring Adage opener vs closer Monitoring vs diagnostics - is it working and how well? Why is it working (not working)? Belt and suspenders: push vs pull is actually push AND pull. Local supervisor vs puppet/ansible setvice start. Run puppet noop
References https://dzone.com/articles/infrastructure-tooling-patterns-list?mz=38541-devops
