# sceptre-playground

learn [sceptre](https://sceptre.cloudreach.com/), a tool to drive cloudformation

* [StackGroup Config](https://sceptre.cloudreach.com/latest/docs/stack_group_config.html) - [`config/dev/config.yaml`](my-sceptre-project/config/dev/config.yaml) - project_code, region, profile, etc.
* [Stack Config](https://sceptre.cloudreach.com/latest/docs/stack_config.html) - [`config/dev/template.yaml`](my-sceptre-project/config/dev/template.yaml) - config for specific stack.  e.g. stack params, template_path, dependencies, hooks, etc.
* Stack - [`templates/template.yaml`](my-sceptre-project/templates/template.yaml)

## Demo

via [Get Started &mdash; Sceptre 2.6.3 documentation](https://sceptre.cloudreach.com/2.6.3/docs/get_started.html)

```sh
# install cli
pipx install sceptre

# create new project
sceptre new project my-sceptre-project

cd my-sceptre-project

# create stack
sceptre create dev/template.yaml

# show stack outputs
sceptre --ignore-dependencies list outputs dev/template.yaml

# update stack
sceptre update dev/template.yaml

# delete stack
sceptre delete dev/template.yaml
```

## Resources

* [sceptre](https://sceptre.cloudreach.com/)
* [Introduction to Sceptre: An AWS Cloudformation Orchestration Tool](https://engineering.carsguide.com.au/introduction-to-sceptre-an-aws-cloudformation-orchestration-tool-4b8453c0ae81)