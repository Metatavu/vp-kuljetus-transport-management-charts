## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

  helm repo add vp-kuljetus https://metatavu.github.io/vp-kuljetus-transport-management-charts

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
vp-kuljetus` to see the charts.

To install the transport-management chart:

    helm install transport-management vp-kuljetus/transport-management

To uninstall the chart:

    helm delete transport-management