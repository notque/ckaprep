# Kubernetes Certified Administration
CKA Prep

* 3 hours
* 24 questions
* Pass mark of 74%
* Remotely proctored
* Chrome browser plus an extension
* Government-issued non-expired ID
* Webcam and microphone
* Clean Work Service (Desk)
* Private Space (no one else in the room)
* Steady internet, preferably 5MB up/down.
* 1-3 Days for Scheduling Exam
* This exam is proctored by a live human but scored by statistical sampling, so if the question asked you to create a Pod with the name of nginx and you created it with the name of web or even nginz, you're not getting points for your attempt even though it may be effectively correct.

* Exam is currently in 1.18, and in September or October will be in 1.19

The latest curriculum can always be found at [https://github.com/cncf/curriculum](https://github.com/cncf/curriculum).

During the exam you are allowed be allowed to open **one** tab apart from the browser based terminal. You can open _any_ link under the [kubernetes.io](kubernetes.io) domain. Some links that will help during the exam are;

* [https://kubernetes.io/docs/reference/kubectl/cheatsheet](https://kubernetes.io/docs/reference/kubectl/cheatsheet)
* [https://discuss.kubernetes.io](https://discuss.kubernetes.io)
* [https://kubernetes.io/docs/home/](https://kubernetes.io/docs/home/)

If you are unsure of the spec or parameters of a yaml, always use `kubectl explain <resource>.<key>`.

## 🛠 Pre-requisites

Time is a big factor, you have **3 hours** to finish **24 questions**. That's **7.5 minutes per question** and they do get progressively harder, so no wasting time on the easier questions. If you’re spending more than 7 mins on questions worth only one or two percent (each question does tell you the percentage it is worth), move on. You won't finish otherwise.

You need to be very comfortable with the following tools, so that you are not wasting time on non task orientated goals.

### tmux

You only get one console, tmux and screen area allowed. This will allow you to split your single console into multiple windows. ie one master, two nodes. Try and use it in your daily workflow to get comfortable with the default settings.

- [ ] **Perform tmux deepdive** - [https://thoughtbot.com/upcase/tmux](https://thoughtbot.com/upcase/tmux) - This course teaches you about tmux's pane and window management, session management, copy-paste, and more. 

### vi

- [ ] **Perform Onramp to Vim** - [https://thoughtbot.com/upcase/onramp-to-vim](https://thoughtbot.com/upcase/onramp-to-vim) - Get up and running with the world's best text editor. No Vim experience is required, but you'll be productive in no time (and blazing-fast, soon).

### systemd

- [ ] Read **Systemd Essentials: Working with Services, Units, and the Journal** and play - [https://www.digitalocean.com/community/tutorials/systemd-essentials-working-with-services-units-and-the-journal](https://www.digitalocean.com/community/tutorials/systemd-essentials-working-with-services-units-and-the-journal) - In this guide, we'll give you a quick run through of the most important commands you'll want to know for managing a systemd enabled server.

- [ ] Read **How To Use Systemctl to Manage Systemd Services and Units** and play - [https://www.digitalocean.com/community/tutorials/how-to-use-systemctl-to-manage-systemd-services-and-units](https://www.digitalocean.com/community/tutorials/how-to-use-systemctl-to-manage-systemd-services-and-units) - In this guide, we will be discussing the systemctl command, which is the central management tool for controlling the init system.

- [ ] Read **How To Use Journalctl to View and Manipulate Systemd Logs** and play - [https://www.digitalocean.com/community/tutorials/how-to-use-journalctl-to-view-and-manipulate-systemd-logs](https://www.digitalocean.com/community/tutorials/how-to-use-journalctl-to-view-and-manipulate-systemd-logs) - In this guide, we will discuss how to use the journalctl utility, which can be used to access and manipulate the data held within the journal.

- [ ] Read **Understanding Systemd Units and Unit Files** and play - [https://www.digitalocean.com/community/tutorials/understanding-systemd-units-and-unit-files](https://www.digitalocean.com/community/tutorials/understanding-systemd-units-and-unit-files) - In this guide, we will introduce you to the different units that systemd can handle..

### kubectl

- [ ] Memorise **kubectl Cheat Sheet** and play - [https://kubernetes.io/docs/reference/kubectl/cheatsheet/](https://kubernetes.io/docs/reference/kubectl/cheatsheet/) - This page is an overview of the kubectl command. **NOTE:** This page can be referenced with your one other available tab.

These aliases will help save the precious time you have. Use these during your studies, so you are used to them on the day.

```sh
alias kc='kubectl'
alias kgp='kubectl get pods'
alias kgs='kubectl get svc'
alias kgc='kubectl get componentstatuses'
alias kctx='kubectl config current-context'
alias kcon='kubectl config use-context'
alias kgc='kubectl config get-context'
```

### openssl/cfssl

- [ ] Memorise **OpenSSL command cheatsheet** and play - [https://www.freecodecamp.org/news/openssl-command-cheatsheet-b441be1e8c4a/](https://www.freecodecamp.org/news/openssl-command-cheatsheet-b441be1e8c4a/) - When it comes to security-related tasks, like generating keys, CSRs, certificates, calculating digests, debugging TLS connections and other tasks related to PKI and HTTPS, you’d most likely end up using the OpenSSL tool.


## 🎯 Practice Test

This following here is great for a testing scenario. It gives you 24 questions to answer, a terminal, and a timer. You bring the cluster and kube config. It's highly suggest running through this to get comfortable with the test environment as this is the best replica for the test environment out there. It uses the same terminal emulator that the test uses, [https://github.com/liftoff/GateOne](https://github.com/liftoff/GateOne).

- [ ] Do **github.com/arush-sal/cka-practice-environment** - [https://github.com/arush-sal/cka-practice-environment](https://github.com/arush-sal/cka-practice-environment) - A sample lab test environment to help in preparation of CKA certification.

- [ ] Do **github.com/stretchcloud/cka-lab-practice** - [https://github.com/stretchcloud/cka-lab-practice](https://github.com/stretchcloud/cka-lab-practice) - A set of exercises that will help you to prepare for the Certified Kubernetes Administrator exam.

- [ ] Read **github.com/dgkanatsios/CKAD-exercises** - [https://github.com/dgkanatsios/CKAD-exercises](https://github.com/dgkanatsios/CKAD-exercises) - A set of exercises to prepare for Certified Kubernetes Application Developer exam by Cloud Native Computing Foundation, some overlap with the above but with more content.

## 🌏 Extra Reading

In case you want for more information about the exam and it's topics, here is another brilliant list of curated resoures that you will find handy.

- [ ] Read **CKA Resources** - [https://gist.github.com/strongjz/4c9ad30a12ab715ae94cf72d0e7bbc30](https://gist.github.com/strongjz/4c9ad30a12ab715ae94cf72d0e7bbc30)
= [ ] Practice Questions - [Practice Questions](https://medium.com/bb-tutorials-and-thoughts/practice-enough-with-these-questions-for-the-ckad-exam-2f42d1228552)
