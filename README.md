# SDK-GO-KTC

Monorepo Go SDK untuk infrastruktur cloud, database, dan layanan enterprise. Dikelola oleh **Kilat Cloud**.

## Daftar SDK

### ☁️ Cloud & Infrastructure
| SDK | Deskripsi |
|-----|-----------|
| **gophercloud** | OpenStack cloud SDK — compute, network, storage, identity |
| **vra-sdk-go** | VMware vRealize Automation (vRA) SDK |
| **cloudflare-go** | Cloudflare API — DNS, CDN, WAF, DDoS protection |
| **lego** | ACME/Let's Encrypt — sertifikat TLS otomatis |
| **go-sdk** | SDK internal Kilat Cloud |

### 🖥️ Server & Hardware Management
| SDK | Deskripsi |
|-----|-----------|
| **go-ipmi** | IPMI — remote server power control & sensor monitoring |
| **go-redfish-api-idrac** | Dell iDRAC Redfish API — server telemetry & management |
| **iDRAC-Telemetry-Reference-Tools** | Dell iDRAC telemetry reference tools |
| **go-proxmox** | Proxmox VE API — virtualisasi KVM/LXC |
| **proxmox-api-go** | Proxmox API client alternatif |
| **go-routeros** | MikroTik RouterOS API — network router management |

### 🗄️ Database SDKs
| SDK | Deskripsi |
|-----|-----------|
| **mongo-go-driver** | MongoDB — document database driver resmi |
| **go-redis** | Redis — in-memory cache & message broker |
| **mysql** | MySQL — relational database driver |
| **go-postgres-rest** | PostgreSQL REST API wrapper |
| **clickhouse-go** | ClickHouse — columnar analytics database |
| **cassandra-gocql-driver** | Apache Cassandra — wide-column NoSQL |
| **go-elasticsearch** | Elasticsearch — search & analytics engine |

### ☁️ Object Storage
| SDK | Deskripsi |
|-----|-----------|
| **minio-go** | MinIO / S3-compatible object storage |
| **go-ceph** | Ceph — distributed storage (RADOS, RBD, CephFS) |

### 💳 Payment Gateways
| SDK | Deskripsi |
|-----|-----------|
| **stripe-go** | Stripe — payment processing internasional |
| **midtrans-go** | Midtrans — payment gateway Indonesia |
| **xendit-go** | Xendit — payment gateway Asia Tenggara |

### 🤖 Messaging & Communication
| SDK | Deskripsi |
|-----|-----------|
| **whatsmeow** | WhatsApp Web API — send/receive messages |

### ☸️ Kubernetes
| SDK | Deskripsi |
|-----|-----------|
| **client-go** | Kubernetes official Go client |

### 🔧 Utilities
| SDK | Deskripsi |
|-----|-----------|
| **rustfst** | Rust finite-state transducer (FST) library — search & NLP |

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
