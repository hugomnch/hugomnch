!pip install pygit2==1.12.2
%cd /content
!git clone https://github.com/lllyasviel/Fooocus.git

%cd /content/Fooocus/models/upscale models/
!wget -0 fooocus_upscaler_s409985e5.bin https://huggingface.co/lllyasviel/misc/resolve/main/fooocus_upscaler_s409985e5.bin?download=true

%cd /content/Fooocus
!python entry_with_update.py --share
