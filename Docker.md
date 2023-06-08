<h1>Docker decrypted</h1>
  <div>
    Hopefully this can shed light onto how to get started fiddling with Docker, while also being capable of explaining to others what you're doing exactly. 
  
  </div>
<h2>What is it?</h2>
<ul>
  <li>
    Docker essentially assigns cubicles (containers) to an office space (the resources) where workers (applications) may conduct tasks.
    The workers are not allowed to use the stapler in the cubicle next door, since they are assigned strictly to their cubicle.
  </li>
  <br>
  <li>
    Docker attaches itself to the OS system on your hardware. It uses the resources provided by the OS of choice to provide the user with the ability to separate your OS into smaller versions of itself.
    These smaller versions are then capable of acting like a new computer, ready to use its logical processing unit for any process/application that the user would like for it to specialize in.
  </li>
  <br>
  <li>
    In contrast, a hypervisor would be directly on top of the hardware. What this means is that for every cubicle (container) that is provisioned, the hypervisor must
  </li>
</ul>
<h2>Pro and Cons</h2>
<ul>
  <li>
    Now with containers, each application does not have to conflict with other applications, whether it be compatibility issues or with hardware.
  </li>
  <br>
  <li>
    The downfall with docker is that windows cannot be run as a container with a linux based docker and vice versa.
  </li>
</ul>
