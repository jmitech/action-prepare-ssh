# action-prepare-ssh

```yaml
- name: Prepare SSH for runner
  uses: jmitech/action-prepare-ssh@v1
  with:
    private_key: ${MY_PRIVATE_KEY}
```

```yaml
- name: Prepare SSH for runner and preload known_hosts
  uses: jmitech/action-prepare-ssh@v1
  with:
    private_key: ${MY_PRIVATE_KEY}
    known_hosts_json_file: deployments.json
```

```yaml
- name: Prepare SSH for runner and preload known_hosts with custom jq query
  uses: jmitech/action-prepare-ssh@v1
  with:
    private_key: ${MY_PRIVATE_KEY}
    known_hosts_json_file: deployments.json
    known_hosts_json_file_jq_query: .hosts
```
