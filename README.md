# src-types.ts
Project file architecture 
import { ReactNode } from 'react';

export interface BentoCardProps {
  id: string;
  title: string;
  subtitle: string;
  size: 'large' | 'medium' | 'small';
  children?: ReactNode;
  onClick: () => void;
}

export interface ActionItem {
  id: string;
  title: string;
  category: string;
  icon: ReactNode;
  shortcut?: string;
  action: () => void;
}
