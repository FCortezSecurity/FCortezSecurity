Hi, I'm Fernando 👋

I'm early in my cybersecurity career, currently focused on breaking into Security Engineering / Cloud Security. I'm still a novice — most of what's here comes from hands-on labs, self-directed projects, and a lot of trial and error rather than years on the job — but I learn by building real things end-to-end and pushing myself to go deeper than a tutorial.

What I'm focused on right now
Designing and hardening cloud environments (AWS/Azure IAM, guardrails, least-privilege architecture)
Detection engineering and validating that controls actually work, not just that they're configured
Understanding security from a business-risk perspective, not just a tooling perspective
A few projects I'd point you to first

meridian-pay-baseline Designed, implemented, and validated AWS security guardrails for a fictional payments company — closing a real privilege-escalation path and confirming the fix against a live AWS account, not just on paper. This is the project that best represents where I'm trying to grow: from finding attacks to designing environments that resist them.

openhound-aws AWS IAM attack-path discovery tool — maps identities, roles, and trust relationships to surface privilege-escalation chains, in the spirit of BloodHound's OpenGraph framework.

detection-engineering-cicd An automated pipeline that simulates real MITRE ATT&CK techniques and validates custom Wazuh detection rules against them, CI/CD-style.

Currently learning / leveling up
Terraform and infrastructure-as-code security patterns
CI/CD security gates (policy-as-code, automated scanning)
Going deeper on cloud-native detection (tying preventive controls to telemetry, not just building them in isolation)
A note on where I'm at

I'd rather be upfront about this than oversell it: I don't have professional Security Engineering experience yet. What I do have is a habit of picking a real problem, building something that actually works, breaking it, fixing it, and writing up what I learned honestly — including where my testing had limits. If that's useful context for you, I'm always open to feedback, conversation, or pointing out where I've got something wrong.

📫 Feel free to reach out or open an issue on any of my repos if something looks interesting or worth discussing.

Content

this is my github portfolio. and i was watching a video on advice about cybersecurity and i came across this part of the video where i feel like i have done more work and focused on the tools rather than on showing how i can take care of a business, what you think? open-source-soc-honeypot Public

PASTED

￢ﾝﾯ localstack start -d __ _______ __ __ / / ____ _________ _/ / ___// /_____ ______/ /__ / / / __ \/ ___/ __ `/ /\__ \/ __/ __ `/ ___/ //_/ / /___/ /_/ / /__/ /_/ / /___/ / /_/ /_/ / /__/ ,< /_____/\____/\___/\__,_/_//____/\__/\__,_/\___/_/

PASTED

￢ﾝﾯ sed -i 's/GATEWAY_LISTEN/LOCALSTACK_GATEWAY_LISTEN/' ~/.bashrc ￢ﾝﾯ localstack status services ￢ﾔﾏ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾳ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾓ ￢ﾔﾃ Service ￢ﾔﾃ Status ￢ﾔﾃ ￢ﾔﾡ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢ﾔﾁ￢

PASTED

terraform plan Terraform used the selected providers to generate the following execution plan. Resource actions are indicated with the following symbols: + create Terraform will perform the following actions: # aws_iam_role.admin will be created + resource "aws_iam_role" "admin" {

PASTED

￢ﾝﾯ terraform apply Terraform used the selected providers to generate the following execution plan. Resource actions are indicated with the following symbols: + create Terraform will perform the following actions: # aws_iam_role.admin will be created + resource "aws_iam_role" "admi

PASTED

￢ﾝﾯ >.... policy = jsonencode({ Version = "2012-10-17" Statement = [ { Effect = "Allow" Action = [ "ecs:UpdateService", "ecs:Describe

PASTED

ls -la total 28 drwxr-xr-x 2 cpt-ferna02 cpt-ferna02 4096 Aug 18 03:22 . drwxr-xr-x 4 cpt-ferna02 cpt-ferna02 4096 Aug 18 03:16 .. -rw-r--r-- 1 cpt-ferna02 cpt-ferna02 6080 Aug 18 03:19 iam.tf -rw-r--r-- 1 cpt-ferna02 cpt-ferna02 555 Aug 18 03:22 outputs.tf -rw-r--r-- 1 cpt-ferna02 cpt-ferna

PASTED

￢ﾝﾯ terraform plan Terraform used the selected providers to generate the following execution plan. Resource actions are indicated with the following symbols: + create Terraform will perform the following actions: # aws_iam_policy.developer_boundary will be created + resource "aws_i

PASTED

terraform destroy aws_iam_user.ci_cd_service_account: Refreshing state... [id=ci-cd-service-account] aws_iam_policy.developer_boundary: Refreshing state... [id=arn:aws:iam::656034208999:policy/developer-permission-boundary] aws_iam_role.ci_cd_deploy: Refreshing state... [id=ci-cd-deploy] aws_ia

PASTED

￢ﾝﾯ cat validation-results.md # Validation Results This document records the evidence for whether the guardrails built in Phase 3 (`guardrails/`) actually close the risks identified in `risk-register.csv`. ## Summary | Risk | Before | After | Status | |---|---|---|---| | R-01 - develope

PASTED

One thing I would change Your README currently says: "Built for $0 using LocalStack..." I understand why you mention it. But I wouldn't make "$0" part of the headline/value proposition. It makes the project sound slightly like: "Look how cheaply I built this." The impressive part isn't the co

PASTED

Yes — and the content of the architecture diagram is strong. Even from the Markdown description, I can see that you're making the diagram tell the same story as the project rather than just making a pretty AWS topology. One thing I would change, though: the diagram itself should show the attack pat

PASTED
