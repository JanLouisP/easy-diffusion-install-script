# easy-diffusion-install-script

Before starting the script create a key pair called webui (rsa) in aws !!!!!!!!!!!!!!!!!!!!!!!

#Takes up to 20 minutes. After its ready you can reach easy-diffusion you need to open a tunnel:
putty -i path\to\your\key.ppk -N -L 9000:127.0.0.1:9000 ubuntu@publicAWSIpAddress

Now you can reach easy-diffusion with: localhost:9000

Some Models, etc form civitai.com: 

Am I real:
wget https://civitai.com/api/download/models/176040 --content-disposition

Virile-reality
wget https://civitai.com/api/download/models/181248 --content-disposition

Copax TimeLessXL
wget https://civitai.com/api/download/models/172160 --content-disposition

Lora:
wget https://civitai.com/api/download/models/152309 --content-disposition


Connect to your ec2 instance an use this: 

while true; do
    cat /var/log/cloud-init-output.log
    sleep 5
done

to check how far the installation is.
