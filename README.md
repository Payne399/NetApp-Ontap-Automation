# OntapAutomationHub
NetApp Ontap Automation, Snapshot, SnapMirror Automation
Usage:
usage: OntapAutomation [-h] [--config <cluster config file>] [--noc] [--seq] [--lic LICENSE] [--key KEY1] [--key2]
                       {config,cluster,ssh,volume,lun,igroup,policy,policy_rule,cifs_share,cifs_access,snapmirror,snapmirror7,snapshot} ...

positional arguments:
  {config,cluster,ssh,volume,lun,igroup,policy,policy_rule,cifs_share,cifs_access,snapmirror,snapmirror7,snapshot}
                        sub-command help
    config              config(credentials) related operation, manage cluster config file include 'add', 'delete', 'show'
    cluster             save configuration by 'getconfig' and manage autosupport/perf-archive by 'autosupport/asup'
    ssh                 run command at remote host via ssh
    volume              manage ontap flexvol: rename,create,delete,modify,etc
    lun                 manage lun: create,delete,modify,map,unmap,etc
    igroup              manage igroup: rename,create,delete,modify,etc
    policy              manage export policy: rename,create,delete,etc
    policy_rule         manage export policy rule: create,delete,modify,etc
    cifs_share          manage cifs share: create,delete,modify,etc
    cifs_access         manage cifs access control(ACL): create,delete,modify,etc
    snapmirror          manage snapmirror:
                        show,monitor,create,initialize,abort,quiesce,break,resync,update,resume,modify,delete,release,reverse_resync,etc
    snapmirror7         manage snapmirror for 7 mode: show,monitor,initialize,abort,quiesce,break,resync,update,resume,release,etc
    snapshot            manage snapshot: show,rename,create,delete,protect,restore,etc

optional arguments:
  -h, --help            show this help message and exit
  --config <cluster config file>
                        the cluster config file path, default: cluster.config in current path, otherwise in app path
  --noc                 no color output, defualt is colored
  --seq                 single thread, execute in the order of input, defualt is multi-threaded
  --lic LICENSE         full path of license file, default: OntapAutomation.lic in current path, otherwise in app path
  --key KEY1            input key to protect cluster config file
  --key2                ask for input key to protect cluster config file
