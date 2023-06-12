Here is the documentation for the `kubectl-view-allocations` plugin:

**kubectl-view-allocations**

The `kubectl-view-allocations` plugin lists resource allocations (such as CPU, memory, GPU, etc.) as defined in the manifest of nodes and running pods. It does not display resource usage like the `kubectl top` command. The plugin allows you to view the allocations in a grouped format, with options to filter the results by namespaces, nodes, pods, and specific resource names.

**Installation:**

To install the `kubectl-view-allocations` plugin, run the following script:

```
curl https://raw.githubusercontent.com/davidB/kubectl-view-allocations/master/scripts/getLatest.sh | bash
```

**Usage:**

To view the available options and usage of the plugin, use the following command:

```
kubectl-view-allocations -h
```

**Examples:**

- Simplest view of resources:
```
kubectl-view-allocations
```

- View CPU and memory utilization:
```
kubectl-view-allocations -u
```

- View only CPU resource usage:
```
kubectl-view-allocations -r cpu
```

- View only memory resource usage:
```
kubectl-view-allocations -r memory
```

- View node-specific usage of memory and CPU:
```
kubectl-view-allocations -g node
```

Note: Replace the resource names (`cpu`, `memory`) with the specific resource you want to filter by.

This documentation provides an overview of the `kubectl-view-allocations` plugin, installation instructions, usage examples, and command-line options.
