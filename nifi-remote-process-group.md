# Nifi remote process group

## make input port discoverable

- Add an input port
    - choose *"receive from: Remote connections (site-to-site)"*
- right click input port
    - *"manage access policies"*
    - choose policy: *"receive data via site-to-site"*
    - add user for external nifi node
- Start input port
- Wait some time while refreshing the remote process group
