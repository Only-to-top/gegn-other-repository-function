# gegn other repository function

```php
use Monitoring\Model\Object_mtx\Object_mtxRepository;

$Object_mtxRepository = new Object_mtxRepository($this->di);
$objects = $Object_mtxRepository->functionName($id_ev);
```

## Query in Repository

```php
use Engine\Core\Database\QueryBuilder;

$queryBuilder = new QueryBuilder();

$sql = $queryBuilder
    ->select('name')
    ->from('mtx_spr_tnpa')
    ->where('id', $act['id_npa'])
    ->sql();

$act_json = $this->db->queryOne($sql, $queryBuilder->values);
```
