<script lang="ts">
    import { Handle, Position, type NodeProps } from '@xyflow/svelte';
   
    let props: NodeProps = $props();


                    

  </script>
   
  <div data-selected={props.selected} class="p-12 bg-white border-black border rounded flex items-center justify-center data-[selected=true]:ring-2">
    <Handle type="target" position={Position.Left} />
    <div class="nodrag">Should not select</div>
    <Handle type="source" position={Position.Right} />
  </div>