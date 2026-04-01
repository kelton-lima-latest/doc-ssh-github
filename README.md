# doc-ssh-github

Gera chaves ssh
```bash
ssh-keygen -t ed25519 -C "user-mail@com.br"
```

Generating public/private ed25519 key pair.
Enter file in which to save the key (/home/user/.ssh/id_ed25519): /home/user/.ssh/empresa  
Created directory '/home/user/.ssh'.
Enter passphrase for "/home/user/.ssh/projeart" (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/user/.ssh/empresa
Your public key has been saved in /home/user/.ssh/empresa.pub
The key fingerprint is:
SHA256:dfhgfdghjfgjhrftyurtyurtyuijtyhjfdgbvhsdfghsdrfg user-mail@com.br
The key's randomart image is:
+--[ED25519 256]--+
|+=o=+            |
|=o==o+           |
|.=+o*o o         |
| .+.o + o      .o|
| . o + oS     o +|
|  . =   o.   . o |
|   o .   o.   E .|
|  oo . . ..  .  .|
| +*o. . .  .. .. |
+----[SHA256]-----+

Ler chave pública
```bash
cat .ssh/empresa.pub
```

Acessar Github
Settings > Deploy Keys > Adicionar título e chave ssh

Configurar conexão ssh

```bash
nano .ssh/config
```

```bash
nano .ssh/config
```

```bash
# conta de trabalho
Host github.com-empresa
        HostName github.com
        User git
        IdentityFile ~/.ssh/empresa
```

