Context: placement + role + enumeration Discussion: https://www.youtube.com/watch?v=AH51NRAWfXs

simple type: node type [api] + enumeration [0001] e.g. api0001 grouped type: node type [api] + cluster id [a] + enumeration [0001] e.g. memcache-a0001 clustered type: cluster name [lb]+ node type [web] + enumeration [0001] e.g. lb-web0001

enumeration has a special case of the run once node in the group. Each dimension has groupings behind it, including placement. The groups can be containment’s/hierarchical, but not necessarily. Placement has 2 main dimensions: location and phase Location:

datacenters (slot, rack, aisle, data center/az, city, region, country)
AWS (placement group, az, vpc, region, account) Phase: dev/wip, ci, integration, qa, test, preprod, staging, prod
ci-usw2-sensu-agent-01

k8s-node-qa-uswest2-01.internal.organization.com

Role: 'k8s-node' Placement: (qa, uswest2, internal) Enumeration: ‘1'

pp-la-sensu-probe-01.internal.organization.com Role: ‘sensu-prod' Placement: (pp, la, internal) Enumeration: ’01'


