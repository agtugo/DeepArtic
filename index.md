## About this 

This is a simple but efficient blog to communicate my ideas. 

## My thoughts about the new M1 Macs

The machines have been released and also the expectations are finally settling or maybe just adjusting. The benchmarks using cinebench are putting this machine in a very interesting place, the single thread is fantastic and the multithread is great for a machine of this price, which I must say is pretty fantastic. There is this perception that mac is expensive, if you compare a 1k USD macbook air with something similar it is a fair price considering the quality of the trackpad, build, monitor and speakears, some people just forget that not everything is just about the electronics is also about the mechanical components of the machine. So according to the benchmarks, there is some thermal throttle, this means that the speed of the processor is reduced in order to reduce the temperature you can check more information in [This - URL](https://youtu.be/S-dOB326mlY?t=432) excelent video, the conclusion is that the performance is reduced in around 15% which let me tell you is not bad at all. So the benefits of getting a macbook pro (MBP) are not so much compared to the macbook air (MBA), the only benefit is the extra battery and a better cooling which apparently is good but the benefit not so much, so you can have the peace of never ever hearing a computer fan again in your house no matter the load, I think that is fantastic.

### M1 for developers. 

#### General 
If you are a developer I think Rosetta2 is doing a fantastic job but it is also not impressive, let me tell you why. X86 emulation has been there for a while, it is very well studied, so translating from a very studied platform to another very studied platform is not something crazy to achieve, it is something similar what happened with the Nintendo Switch emulators like Yuzu they reached a progress in no time, and the reason is the architecure of a Nintendo switch was very similar to the mobile devices we have today, so making an emulator was not that difficult compared to making a n64 emulator. Since x86 apps are running great is not crazy to think that also virtualization of x86 run greats, I am not a apple user (only my ipad) but I am becoming one and it is important to notice the following. You are not getting eGPU acceleration (anyway there are no Nvidia support on mac) so this means no ML at least not with the most known and popular platforms. Apple mentioned that it would be possible to use tensorflow but I hightly doubt that this will be for training, this is just clearly for inference but of course we need to wait for confirmation in that matter. Ok let's talk about price, the model base is great! but if you want to add just a little ssd and ram. Are they crazy? 200 hundred dollars for 8gb more of RAM? 16GB should be the standard for "PRO" anyway. I cannot imagine running a virtual machine, emulating a smartphone with 8GB of RAM. I know apple says is about the experience and everything, but if you need to save 4GB of RAM for a process how the "experience" is going to save you. It is something that you can compensate with a efficiente operating system and well developed apps, but some processes specially data science when you cannot just compensate without developing time cost. 

#### Docker
Docker with linux is not working. Period. The end. Just jocking it is not working now but docker is workinf to deliver a version for this. So not yet but soon. 

#### Servers
Ok When we test, when we code in general the target platform is the same than the machine used to develop. Almost all the servers are x86. So, what are the options? cross-compilation? emulation? Or maybe we are going to see a tendency for arm severs. Anyway alot of code nowadays is for virtual machines and interpreters, so maybe there won't be a lot of changes in that sense but I really believe what Torvalds said about why we don't have arm servers (the reason I explained). So we'll see. 

```markdown
print("Bye world")
```
