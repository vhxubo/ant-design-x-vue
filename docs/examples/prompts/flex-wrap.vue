<script setup lang="tsx">
import { BulbOutlined, CheckCircleOutlined, CoffeeOutlined, FireOutlined, InfoCircleOutlined, RocketOutlined, SmileOutlined, WarningOutlined } from '@ant-design/icons-vue';
import { Prompts, type PromptsProps } from 'ant-design-x-vue';


defineOptions({ name: 'AXPromptsFlexWrap' });

const items: PromptsProps['items'] = [
  {
    key: '1',
    icon: <BulbOutlined style={{ color: '#FFD700' }} />,
    description: 'Got any sparks for a new project?',
  },
  {
    key: '2',
    icon: <InfoCircleOutlined style={{ color: '#1890FF' }} />,
    description: 'Help me understand the background of this topic.',
  },
  {
    key: '3',
    icon: <WarningOutlined style={{ color: '#FF4D4F' }} />,
    description: 'How to solve common issues? Share some tips!',
  },
  {
    key: '4',
    icon: <RocketOutlined style={{ color: '#722ED1' }} />,
    description: 'How can I work faster and better?',
  },
  {
    key: '5',
    icon: <CheckCircleOutlined style={{ color: '#52C41A' }} />,
    description: 'What are some tricks for getting tasks done?',
  },
  {
    key: '6',
    icon: <CoffeeOutlined style={{ color: '#964B00' }} />,
    description: 'How to rest effectively after long hours of work?',
  },
  {
    key: '7',
    icon: <SmileOutlined style={{ color: '#FAAD14' }} />,
    description: 'What are the secrets to maintaining a positive mindset?',
  },
  {
    key: '8',
    icon: <FireOutlined style={{ color: '#FF4D4F' }} />,
    description: 'How to stay calm under immense pressure?',
  },
];

defineRender(() => {
  return (
    <Prompts title="✨ Inspirational Sparks and Marvelous Tips" items={items} wrap />
  )
});
</script>
