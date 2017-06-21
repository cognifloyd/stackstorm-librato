# Librato Integration Pack

This pack allows for Librato integrations.

## Configuration

Copy the example configuration in [librato.yaml.example](./librato.yaml.example)
to `/opt/stackstorm/configs/librato.yaml` and edit as required.

It must contain:

* ``user`` - Librato token
* ``token`` - Librato token

You can also use dynamic values from the datastore. See the
[docs](https://docs.stackstorm.com/reference/pack_configs.html) for more info.

**Note** : When modifying the configuration in `/opt/stackstorm/configs/` please
           remember to tell StackStorm to load these new values by running
           `st2ctl reload --register-configs`

## Actions

* ``add_annotation``
* ``delete_metric``
* ``get_metric``
* ``list_metrics``
* ``submit_counter``
* ``submit_gauge``
