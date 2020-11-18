## About this 

Follow me on twitter: @DeepArtic. This is a simple but efficient blog to communicate my ideas. 

## My thoughts about the new M1 Macs

The machines have been released and also the expectations are finally settling or maybe just adjusting. So if you are not familiar with the change apple is changing to __x86__ processors to __ARM__ processors. For comparison this is similar to going from gasoline to diesel, different engine, different process and more or less the same result. The benchmarks using cinebench are putting this machine in a very interesting place, the **single thread** is fantastic and the **multithread is great for a machine** of this price and size, which I must say is pretty fantastic. There is this perception that mac is expensive, if you compare a **1k USD macbook air** with something similar it is a good price considering the quality of the trackpad, build quality, monitor and speakers, some people just forget that not everything is just about the electronics is also about the mechanical components of the machine. Also it's worth to mention that flagship windows laptops start at **2k USD**.

So according to the benchmarks, there is some thermal throttle, this means that the speed of the processor is reduced in order to reduce the temperature you can check more information in **[this](https://youtu.be/S-dOB326mlY?t=432)** excelent video, the conclusion is that the performance is reduced in around 15% which let me tell you is not bad at all. So the __benefits of getting a macbook pro (MBP) are not so much compared to the macbook air (MBA)__, the only benefit is the extra battery and a better cooling which apparently is good but the benefit not so much, and with a MBA you can have the peace of never ever hearing a computer fan again in your house no matter the load, I think that is fantastic. I forgot to mention the macbook air doesn't have the **horrible touch bar**. So as you can see the decision is difficult.  

### M1 for developers. 

#### General 
If you are a developer I think __Rosetta2 is doing a fantastic job__ but it is also not impressive, let me tell you why. X86 emulation has been there for a while, it is very well studied, so translating from a very studied platform to another very studied platform is not something crazy to achieve, it is something similar what happened with the Nintendo Switch emulators like Yuzu they reached a progress in no time, and the reason is the architecure of a Nintendo switch was very similar to the mobile devices we have today, so making an emulator was not that difficult compared to making a n64 emulator. Since x86 apps are running great is not crazy to think that also virtualization of x86 run great also (available?), I am not a apple user (only my ipad) but I am becoming one and it is important to notice the following. You are **not** getting eGPU acceleration over thunderbolt 4 (anyway there are no Nvidia support on mac) so this means no Machine/Deep Learning at least not with the most known and popular platforms. 

Apple mentioned that it would be possible to use tensorflow but I hightly doubt that will be for training, this is just clearly for inference but of course we need to wait for confirmation in that matter. Ok let's talk about price, the base model is great! but if you want to add just a little ssd and ram - Are they crazy? **200 hundred dollars for 8gb** more of RAM? - 16GB should be the standard for "PRO" anyway. I cannot imagine running a virtual machine, emulating a smartphone with 8GB of RAM. I know apple says is about the experience and stuff, but if you need to save 4GB of RAM for a process how the "experience" is going to save you. I mean less RAM , it is something that you can compensate with a efficient operating system and well developed apps, but some processes specially data science you cannot just compensate without developing time which at the end is money.

#### Docker
**Docker with linux is not working**. Period. The end. Just jocking it is not working now but docker is working to deliver a version for this. So not yet but soon. 

#### Servers

Ok, when we code in general the target platform is the same than the machine used to develop. Almost all the servers are x86. So, what are the options? cross-compilation? emulation? docker? are we going to see a tendency to use ARM for severs? Anyway a lot of code nowadays is for virtual machines (example: java) and interpreters, so maybe there won't be a lot of changes in that sense but I really believe what __Torvalds said about why we don't have arm servers is because we do not have ARM PCs__. I think in the worst case scenario we just create a linux virtual machine ( do not forget the extra RAM and extra SSD) and develop there.

```markdown
print("Bye world")
```
