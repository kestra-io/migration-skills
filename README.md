⚠️ Archived and moved to [agent-skills](https://github.com/kestra-io/agent-skills/pull/4)

# migration-skills

Claude Code skills for migrating workflows to [Kestra](https://kestra.io).

## Skills

| Skill | Description |
|---|---|
| [migrate-airflow-kestra](./migrate-airflow-kestra/SKILL.md) | Migrate an Airflow DAG to a production-ready Kestra flow. Extracts Python task logic into namespace files, maps DAG dependencies to Kestra tasks, and preserves parallel execution structure. |

## Usage

Skills are loaded by Claude Code from `~/.claude/skills/`. To use a skill from this repo, symlink the directory:

```bash
ln -s /path/to/migration-skills/migrate-airflow-kestra ~/.claude/skills/migrate-airflow-kestra
```

Then invoke it in Claude Code:

```
/migrate-airflow-kestra dags/my_dag.py kestra/
```
