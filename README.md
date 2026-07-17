# SDK-GO-KTC

Monorepo Go SDK untuk infrastruktur cloud, database, dan layanan enterprise. Dikelola oleh **Kilat Cloud**.

## Daftar SDK

### ☁️ Cloud & Infrastructure
| SDK | Deskripsi | Repo Asli |
|-----|-----------|-----------|
| **gophercloud** | OpenStack cloud SDK — compute, network, storage, identity | [kilat-cloud/gophercloud](https://github.com/kilat-cloud/gophercloud) |
| **vra-sdk-go** | VMware vRealize Automation (vRA) SDK | [kilat-cloud/vra-sdk-go](https://github.com/kilat-cloud/vra-sdk-go) |
| **cloudflare-go** | Cloudflare API — DNS, CDN, WAF, DDoS protection | [kilat-cloud/cloudflare-go](https://github.com/kilat-cloud/cloudflare-go) |
| **lego** | ACME/Let's Encrypt — sertifikat TLS otomatis | [kilat-cloud/lego](https://github.com/kilat-cloud/lego) |
| **go-sdk** | SDK internal Kilat Cloud | [kilat-cloud/go-sdk](https://github.com/kilat-cloud/go-sdk) |

### 🖥️ Server & Hardware Management
| SDK | Deskripsi | Repo Asli |
|-----|-----------|-----------|
| **go-ipmi** | IPMI — remote server power control & sensor monitoring | [kilat-cloud/go-ipmi](https://github.com/kilat-cloud/go-ipmi) |
| **go-redfish-api-idrac** | Dell iDRAC Redfish API — server telemetry & management | [kilat-cloud/go-redfish-api-idrac](https://github.com/kilat-cloud/go-redfish-api-idrac) |
| **iDRAC-Telemetry-Reference-Tools** | Dell iDRAC telemetry reference tools | [kilat-cloud/iDRAC-Telemetry-Reference-Tools](https://github.com/kilat-cloud/iDRAC-Telemetry-Reference-Tools) |
| **go-proxmox** | Proxmox VE API — virtualisasi KVM/LXC | [kilat-cloud/go-proxmox](https://github.com/kilat-cloud/go-proxmox) |
| **proxmox-api-go** | Proxmox API client alternatif | [kilat-cloud/proxmox-api-go](https://github.com/kilat-cloud/proxmox-api-go) |
| **go-routeros** | MikroTik RouterOS API — network router management | [kilat-cloud/go-routeros](https://github.com/kilat-cloud/go-routeros) |

### 🗄️ Database SDKs
| SDK | Deskripsi | Repo Asli |
|-----|-----------|-----------|
| **mongo-go-driver** | MongoDB — document database driver resmi | [kilat-cloud/mongo-go-driver](https://github.com/kilat-cloud/mongo-go-driver) |
| **go-redis** | Redis — in-memory cache & message broker | [kilat-cloud/go-redis](https://github.com/kilat-cloud/go-redis) |
| **mysql** | MySQL — relational database driver | [kilat-cloud/mysql](https://github.com/kilat-cloud/mysql) |
| **go-postgres-rest** | PostgreSQL REST API wrapper | [kilat-cloud/go-postgres-rest](https://github.com/kilat-cloud/go-postgres-rest) |
| **clickhouse-go** | ClickHouse — columnar analytics database | [kilat-cloud/clickhouse-go](https://github.com/kilat-cloud/clickhouse-go) |
| **cassandra-gocql-driver** | Apache Cassandra — wide-column NoSQL | [kilat-cloud/cassandra-gocql-driver](https://github.com/kilat-cloud/cassandra-gocql-driver) |
| **go-elasticsearch** | Elasticsearch — search & analytics engine | [kilat-cloud/go-elasticsearch](https://github.com/kilat-cloud/go-elasticsearch) |

### ☁️ Object Storage
| SDK | Deskripsi | Repo Asli |
|-----|-----------|-----------|
| **minio-go** | MinIO / S3-compatible object storage | [kilat-cloud/minio-go](https://github.com/kilat-cloud/minio-go) |
| **go-ceph** | Ceph — distributed storage (RADOS, RBD, CephFS) | [kilat-cloud/go-ceph](https://github.com/kilat-cloud/go-ceph) |

### 💳 Payment Gateways
| SDK | Deskripsi | Repo Asli |
|-----|-----------|-----------|
| **stripe-go** | Stripe — payment processing internasional | [kilat-cloud/stripe-go](https://github.com/kilat-cloud/stripe-go) |
| **midtrans-go** | Midtrans — payment gateway Indonesia | [kilat-cloud/midtrans-go](https://github.com/kilat-cloud/midtrans-go) |
| **xendit-go** | Xendit — payment gateway Asia Tenggara | [kilat-cloud/xendit-go](https://github.com/kilat-cloud/xendit-go) |

### 🤖 Messaging & Communication
| SDK | Deskripsi | Repo Asli |
|-----|-----------|-----------|
| **whatsmeow** | WhatsApp Web API — send/receive messages | [kilat-cloud/whatsmeow](https://github.com/kilat-cloud/whatsmeow) |

### ☸️ Kubernetes
| SDK | Deskripsi | Repo Asli |
|-----|-----------|-----------|
| **client-go** | Kubernetes official Go client | [kilat-cloud/client-go](https://github.com/kilat-cloud/client-go) |

### 🔧 Utilities
| SDK | Deskripsi | Repo Asli |
|-----|-----------|-----------|
| **rustfst** | Rust finite-state transducer (FST) library — search & NLP | [kilat-cloud/rustfst](https://github.com/kilat-cloud/rustfst) |

## Struktur

```
SDK-GO-KTC/
├── gophercloud/          # OpenStack
├── vra-sdk-go/           # VMware vRA
├── cloudflare-go/        # Cloudflare
├── lego/                 # TLS/ACME
├── go-sdk/               # SDK internal
├── go-ipmi/              # IPMI
├── go-proxmox/           # Proxmox
├── go-routeros/          # MikroTik
├── mongo-go-driver/      # MongoDB
├── go-redis/             # Redis
├── mysql/                # MySQL
├── clickhouse-go/        # ClickHouse
├── go-elasticsearch/     # Elasticsearch
├── minio-go/             # MinIO/S3
├── stripe-go/            # Stripe
├── midtrans-go/          # Midtrans
├── xendit-go/            # Xendit
├── whatsmeow/            # WhatsApp
├── client-go/            # Kubernetes
├── go-ceph/              # Ceph
├── cassandra-gocql-driver/ # Cassandra
├── go-postgres-rest/     # PostgreSQL REST
├── go-redfish-api-idrac/ # Dell iDRAC
├── iDRAC-Telemetry-Reference-Tools/ # Dell telemetry
├── rustfst/              # FST library
└── ...
```

## Penggunaan

Import langsung dari monorepo:

```go
import "github.com/kilat-cloud/SDK-GO-KTC/gophercloud"
```

Atau gunakan `go.work` untuk development lokal:

```bash
go work init
go work use ./gophercloud ./go-redis ./minio-go
```

## Lisensi

Masing-masing SDK memiliki lisensinya sendiri sesuai repo upstream.
