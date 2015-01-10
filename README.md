zafar.cc
========
## Setting up the current repo
1. [Install Bower](http://bower.io/#install-bower)
2. Run `bower install` in the root directory
3. Create your own HTML pages
4. Add links to your pages in the main `index.html` (just follow the template in there)

## Running a web server on Amazon AWS
### Preliminaries

#### Create security group: SSH/HTTP/HTTPS access to EC2
![Create Security Group][amazonSecurity1]

#### Create new EC2 instance
![Create New Instance][amazonInstance1]

#### Follow the "new instance wizard" steps
1. Choose an Amazon Image (Free tier Ubuntu Server 64-bit)
2. Choose an instance type (Free tier micro)
3. Configure instance (defaults)
4. Configure storage (General purpose SSD - 10GiB)
5. Tag instance (Anything)
6. Choose the security settings for the new instance
![Pick the instance security][amazonInstance2]

#### Launch the instance
After clicking on `Launch` you will need to create/select a new key pair, 
download it, and place it under `~/.ssh/` directory

<img 
  src="https://www.dropbox.com/s/4wqyg8wf9j35io5/amazonInstance3.png?dl=1"
  height="400px" 
/>

[amazonSecurity1]: https://www.dropbox.com/s/04greovza207p7m/amazonSecurity1.png?dl=1 "Create new security group"
[amazonInstance1]: https://www.dropbox.com/s/55fazphx06y77t1/amazonInstance1.png?dl=1 "Create new instance"
[amazonInstance2]: https://www.dropbox.com/s/keptddjcdod1j6z/amazonInstance2.png?dl=1 "Select security for the new instance"
[amazonInstance3]: https://www.dropbox.com/s/4wqyg8wf9j35io5/amazonInstance3.png?dl=1 "Create license key"
