---
last_modified: 2015/07/16
translation_status: complete
language: ja
title: Datadog-HAProxy Integration
integration_title: HAProxy
git_integration_title: haproxy
kind: integration
doclevel: complete
---

<!-- ## Overview

Capture HAProxy activity in Datadog to:

- Visualize HAProxy load-balancing performance.
- Know when a server goes down.
-  Correlate the performance of HAProxy with the rest of your applications. -->

## 概要

次の目的で、HAProxyの動作状況をDatadogと連携します:

* HAProxyのロードバランシングパフォーマンスの可視化
* HAProxyサーバーがダウンしたことを検知する
* HAProxyのパフォーマンスと他のアプルケーションの情報を関連付けて把握する

Datadog Agentの設定ファイルサンプルとメトリクス取得プログラム:

* [HAProxyインテグレーションの設定ファイルサンプル](https://github.com/DataDog/integrations-core/blob/master/haproxy/conf.yaml.example)
* [HAProxyインテグレーション checks.d](https://github.com/DataDog/integrations-core/blob/master/haproxy/datadog_checks/haproxy/haproxy.py)

<!-- The following metrics are collected by default with the HAProxy integration:

    haproxy.bytes.in_rate
    haproxy.bytes.out_rate
    haproxy.denied.req_rate
    haproxy.denied.resp_rate
    haproxy.errors.con_rate
    haproxy.errors.req_rate
    haproxy.errors.resp_rate
    haproxy.queue.current
    haproxy.requests.rate
    haproxy.session.current
    haproxy.session.limit
    haproxy.session.rate
    haproxy.warnings.redis_rate
    haproxy.warnings.retr_rate -->

HAProxyインテグレーションがデフォルトで取得しているメトリクス:

    haproxy.bytes.in_rate
    haproxy.bytes.out_rate
    haproxy.denied.req_rate
    haproxy.denied.resp_rate
    haproxy.errors.con_rate
    haproxy.errors.req_rate
    haproxy.errors.resp_rate
    haproxy.queue.current
    haproxy.requests.rate
    haproxy.session.current
    haproxy.session.limit
    haproxy.session.rate
    haproxy.warnings.redis_rate
    haproxy.warnings.retr_rate
