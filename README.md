# Useful DockerFiles For Deployment of VPN Servers

Useful Repositories as Submodules to Deploy on Server.
Repositories are Listed as Below:
 - MTProxy (Telegram Messenger)
 - Pritunl (OpenVPN Based With GUI Server)

## Additional Instructions

### MTProxy
Change `--http-port` inside Dockerfile **CMD**  command to change Proxy Port`
### Pritunl 
Add Latest Version Of Pritunl in `docker-install.sh` to avoid download error

After Setting Up Docker Container. in Case Of Having Issue Logging in for the First time Attach To Container Using `docker exec -ti --privileged <Container-Name-ir-ID> bash` and use following Command :
`pritunl reset-password`

Login With New Credentials.

After Setting Up For The First time You can Attach A Domain For SSL Console Web Page By Providing Domain Name in `Lets Encrypt Domain` Field in Setting

Make Sure the Port Specified for Server Has been Exposed To outside of Docker Environment

