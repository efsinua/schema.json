# kind.x-k8s.io.schema.json

Compatible with vscode validators JSON Shema for [kind - https://kind.sigs.k8s.io)](https://kind.sigs.k8s.io/) YAML config.

See for mote details:

[https://github.com/kubernetes-sigs/kind/](https://github.com/kubernetes-sigs/kind/)

[https://github.com/kubernetes-sigs/kind/blob/main/pkg/apis/config/v1alpha4/types.go](https://github.com/kubernetes-sigs/kind/blob/main/pkg/apis/config/v1alpha4/types.go)

Assuming you're using ms-kubernetes-tools.vscode-kubernetes-tools plugin.

Add this to you workspace file:

	{
		"settings": {
			"yaml.schemas": {
				"Kubernetes": [
					"*.kubernetes.yaml",
					"*.k8s.yaml",
					"*.kapi.yaml",
					"*!(.kind).cluster.yaml",
					"*.capi.yaml"
				],
				"https://raw.githubusercontent.com/efsinua/schema.json/main/kind.x-k8s.io.schema.json": [
					"*.kind.yaml",
					"*.kind.cluster.yaml"
				]
			}
		}
	}