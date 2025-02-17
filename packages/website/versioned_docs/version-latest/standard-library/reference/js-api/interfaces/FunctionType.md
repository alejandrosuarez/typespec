---
jsApi: true
title: "[I] FunctionType"

---
## Extends

- [`BaseType`](BaseType.md)

## Properties

| Property | Type | Description | Inheritance |
| :------ | :------ | :------ | :------ |
| `implementation` | (...`args`) => `unknown` | - | - |
| `instantiationParameters?` | [`Type`](../type-aliases/Type.md)[] | - | [`BaseType.instantiationParameters`](BaseType.md) |
| `isFinished` | `boolean` | Reflect if a type has been finished(Decorators have been called).<br />There is multiple reasons a type might not be finished:<br />- a template declaration will not<br />- a template instance that argument that are still template parameters<br />- a template instance that is only partially instantiated(like a templated operation inside a templated interface) | [`BaseType.isFinished`](BaseType.md) |
| `kind` | `"Function"` | - | [`BaseType.kind`](BaseType.md) |
| `name` | `string` | - | - |
| `namespace?` | [`Namespace`](Namespace.md) | - | - |
| `node?` | [`FunctionDeclarationStatementNode`](FunctionDeclarationStatementNode.md) | - | [`BaseType.node`](BaseType.md) |
| `parameters` | [`FunctionParameter`](FunctionParameter.md)[] | - | - |
| `projectionBase?` | [`Type`](../type-aliases/Type.md) | - | [`BaseType.projectionBase`](BaseType.md) |
| `projectionSource?` | [`Type`](../type-aliases/Type.md) | - | [`BaseType.projectionSource`](BaseType.md) |
| `projector?` | [`Projector`](Projector.md) | - | [`BaseType.projector`](BaseType.md) |
| `returnType` | [`Type`](../type-aliases/Type.md) | - | - |

## Accessors

### projections

```ts
get projections(): ProjectionStatementNode[]
```

#### Returns

[`ProjectionStatementNode`](ProjectionStatementNode.md)[]

## Methods

### projectionsByName()

```ts
projectionsByName(name): ProjectionStatementNode[]
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

[`ProjectionStatementNode`](ProjectionStatementNode.md)[]

#### Inherited from

[`BaseType.projectionsByName`](BaseType.md#projectionsbyname)
