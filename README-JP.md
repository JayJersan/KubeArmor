![KubeArmor Logo](.gitbook/assets/logo.png)

[![Build Status](https://github.com/kubearmor/KubeArmor/actions/workflows/ci-go.yml/badge.svg)](https://github.com/kubearmor/KubeArmor/actions/workflows/ci-go.yml/)
[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5401/badge)](https://bestpractices.coreinfrastructure.org/projects/5401)
[![Slack](https://img.shields.io/badge/Join%20Our%20Community-Slack-blue)](https://join.slack.com/t/kubearmor/shared_invite/zt-1ltmqdbc6-rSHw~LM6MesZZasmP2hAcA)
[![Discussions](https://img.shields.io/badge/Got%20Questions%3F-Chat-Violet)](https://github.com/kubearmor/KubeArmor/discussions)

[English](README.md)

KubeArmor は、ポッド、コンテナー、およびノー​​ド (VM) の動作 \(プロセス実行、ファイル アクセス、ネットワーク操作など\) をシステム レベルで制限する、クラウドネイティブのランタイム セキュリティ強制システムです。
KubeArmor は、 [AppArmor](https://en.wikipedia.org/wiki/AppArmor), [SELinux](https://en.wikipedia.org/wiki/Security-Enhanced_Linux), or [BPF-LSM](https://docs.kernel.org/bpf/prog_lsm.html)　などの [Linux security modules \(LSMs\)](https://en.wikipedia.org/wiki/Linux_Security_Modules) を活用して、ユーザー指定のポリシーを強制します。 KubeArmor は、eBPF を活用して、コンテナー/ポッド/名前空間 ID を使用して豊富なアラート/テレメトリ イベントを生成します

|  |   |
|:---|:---|
| :muscle: **[インフラの強化](getting-started/hardening_guide.md)** <hr>:chains: 証明書バンドルなどのクリティカルパスを保護 <br>:clamp: MITRE、STIG、CIS ベースのルール <br>:left_luggage: 生の DB テーブルへのアクセスを制限 | :ring: **[最も許容度の低いアクセス](getting-started/least_permissive_access.md)** <hr>:traffic_light: プロセスのホワイトリスト <br>:traffic_light: ネットワークのホワイトリスト <br>:control_knobs: 機密アセットへのアクセスを制御 |
| :telescope: **[アプリケーションの動作](getting-started/workload_visibility.md)** <hr>:dna: プロセス実行、ファイル システム アクセス <br>:compass: サービスバインド、イングレス接続、エグレス接続 <br>:microscope: 機密性の高いシステムコール | :snowflake: **[デプロイメント モデル](getting-started/deployment_models.md)** <hr>:wheel_of_dharma: Kubernetes デプロイメント<br>:whale2: コンテナ デプロイメント<br>:desktop_computer: VM/ベアメタル デプロイメント |

## アーキテクチャの概要

![KubeArmor High Level Design](.gitbook/assets/kubearmor_overview.png)

## ドキュメンテーション :notebook:

* :point_right: [入門](getting-started/deployment_guide.md)
* :dart: [ユースケース](getting-started/use-cases.md)
* :heavy_check_mark: [KubeArmor サポート マトリックス](getting-started/support_matrix.md)
* :medal_sports: [KubeArmorの違いは?](getting-started/differentiation.md)
* :scroll: ポッド/コンテナのセキュリティ ポリシー [[Spec](getting-started/security_policy_specification.md)] [[Examples](getting-started/security_policy_examples.md)]
* :scroll: ホスト/ノードのセキュリティ ポリシー [[Spec](getting-started/host_security_policy_specification.md)] [[Examples](getting-started/host_security_policy_examples.md)]

### Contributors :busts_in_silhouette:

* :octocat: [Contribution Guide](contribution/contribution_guide.md)
* :technologist: [Development Guide](contribution/development_guide.md), [Testing Guide](contribution/testing_guide.md)
* :raising_hand_woman: [Join KubeArmor Slack](https://join.slack.com/t/kubearmor/shared_invite/zt-1ltmqdbc6-rSHw~LM6MesZZasmP2hAcA)
* :question: [FAQs](getting-started/FAQ.md)

### Biweekly Meetup

- :speaking_head: [Zoom Link](http://zoom.kubearmor.io)
- :page_facing_up: Minutes: [Document](https://docs.google.com/document/d/1IqIIG9Vz-PYpbUwrH0u99KYEM1mtnYe6BHrson4NqEs/edit)
- :calendar: Calendar invite: [Google Calendar](http://www.google.com/calendar/event?action=TEMPLATE&dates=20220210T150000Z%2F20220210T153000Z&text=KubeArmor%20Community%20Call&location=&details=%3Ca%20href%3D%22https%3A%2F%2Fdocs.google.com%2Fdocument%2Fd%2F1IqIIG9Vz-PYpbUwrH0u99KYEM1mtnYe6BHrson4NqEs%2Fedit%22%3EMinutes%20of%20Meeting%3C%2Fa%3E%0A%0A%3Ca%20href%3D%22%20http%3A%2F%2Fzoom.kubearmor.io%22%3EZoom%20Link%3C%2Fa%3E&recur=RRULE:FREQ=WEEKLY;INTERVAL=2;BYDAY=TH&ctz=Asia/Calcutta), [ICS file](getting-started/resources/KubeArmorMeetup.ics)

## 注意事項/クレジット :handshake:

- KubeArmorは[Tracee](https://github.com/aquasecurity/tracee/)のシステムコールユーティリティ関数を使っています.

## CNCF

KubeArmorはCloud Native Computing Foundationの[Sandbox Project](https://www.cncf.io/projects/kubearmor/)です.
![CNCF SandBox Project](.gitbook/assets/cncf-sandbox.png)